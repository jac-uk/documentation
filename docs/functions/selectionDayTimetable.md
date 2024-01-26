### Input Data Models

1.  **Panel:**
    -   `panel`: Object
        -   `id`: string
    -   `panellists`: Array of Objects
        -   `id`: string
    -   `date`: Date
    -   `totalSlots`: number
2.  **Candidate Info:**
    -   `candidate`: Object
        -   `id`: string
    -   `availableDates`: Array of Date
3.  **Reasonable Adjustments:**
    -   `reasonableAdjustments`: Array of strings (candidate IDs)
4.  **Panel Conflicts:**
    -   `panelConflicts`: Array of Objects
        -   `candidate`: Object
            -   `id`: string
        -   `panellist`: Object
            -   `id`: string

### Output Data Models

1.  **Timetable Data Model:**
    -   `timetable`: Array of Objects
        -   `candidateRef`: string (candidate ID)
        -   `date`: Date
        -   `panel`: string (panel ID)
        -   `reasonableAdjustment`: boolean
        -   `slot`: number
2.  **Unassigned Candidates Data Model:**
    -   `unassignedCandidates`: Array of Objects
        -   `candidate`: Object
            -   `id`: string
        -   `availableDates`: Array of Date

### Examples:

#### Input Example:
```
const panelData = [
  {
    panel: { id: 'panel1' },
    panellists: [{ id: 'panellist1' }],
    date: new Date('2024-01-01'),
    totalSlots: 3,
  },
  // ... other panels
];

const candidateInfo = [
  {
    candidate: { id: 'candidate1' },
    availableDates: [new Date('2024-01-01'), new Date('2024-01-02')],
  },
  // ... other candidates
];

const reasonableAdjustments = ['candidate2', 'candidate4'];

const panelConflicts = [
  {
    candidate: { id: 'candidate3' },
    panellist: { id: 'panellist1' },
  },
  // ... other conflicts
];

selectionDayTimetable(panelData, candidateInfo, reasonableAdjustments, panelConflicts);
```
#### Output Example:
```
{
  timetable: [
    { CandidateRef: 'candidate1', Date: new Date('2024-01-01'), Panel: 'panel1', ReasonableAdjustment: true, Slot: 1 },
    // ... other timetable entries
  ],
  unassignedCandidates: [
    { candidate: { id: 'candidate5' }, availableDates: [new Date('2024-01-01')] },
    // ... other unassigned candidates
  ],
}

```

**Overview:**
   - The `selectionDayTimetable` function manages the scheduling of candidates for panels on specific dates.

**Input Parameters:**
   - The function takes four main inputs:
     - `panelData`: Information about panels, including their ID, panellists, date, and the total available slots.
     - `candidateInfo`: Details about candidates, such as their ID and the dates they are available for.
     - `reasonableAdjustments`: A list of candidate IDs eligible for reasonable adjustments.
     - `panelConflicts`: Information about conflicts between candidates and panellists on specific panels.

**Timetable Generation:**
   - The function generates a timetable that assigns candidates to panels on available dates.
   - For each panel, it assigns candidates based on their availability and the total available slots.

The function achieves this in 5 main steps

 1. Matching 'suitable' Candidates to panels and matching 'suitable' panels to candidates.
 2. Assign candidates with only one 'suitable' panel to a slot 
 3. Assign candidates with more than one 'suitable' panel to a slot
 4. Collect a list of the unassigned candidates
 5. Output the result

**Reasonable Adjustments:**
    - Candidates eligible for reasonable adjustments are given priority in the assignment process.
    - These candidates are flagged in the timetable to indicate they received special considerations.

**Handling Conflicts:**
    - The function considers conflicts between candidates and panellists on specific panels.
    - Candidates with conflicts are appropriately handled to ensure fair and conflict-free assignments.

**Output:**
   - The function produces a timetable with details such as the candidate reference, date, panel ID, reasonable adjustment status, and assigned slot.
   - Additionally, it provides a list of unassigned candidates with their details.

**Edge Cases:**
   - The function accounts for various scenarios, including no available candidates, no panels, no conflicts, and a combination of conflicts and reasonable adjustments.
   - It handles performance testing with larger datasets efficiently.

**Conclusion:**
   - `selectionDayTimetable` assigns candidates to panels while considering conflicts and listing reasonable adjustments, aiming to fill the most slots possible.
