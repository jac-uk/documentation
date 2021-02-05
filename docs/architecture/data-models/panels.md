# Data Model: Panels

## Collection: Panels
A `Panels` document contains the following fields:
```
  exerciseId: String,
  name: String,
  type: String ('sift', 'selection'),
  members: [ { fullName: String, email: String, phone: String, title: String } ],
  status: String ('draft', 'created', 'completed'),
```

## Relationship: Panels and ApplicationRecords
The following fields are added to the `ApplicationRecords` document in order to store the relationship with `Panels`.
```
  panelIds: {
    sift: String,  // Id of Panels document of type 'sift'
    selection: String,  // Id of Panels document of type 'selection'
  }
```
Each `type` of panel will have an entry in the `panelIds` map. These entries will be initialised to an empty string (to indicate the application has not been assigned to a panel) and eventually assigned the `id` of a `Panels` document.
Initialising the `panelIds` map will happen when the respective panel task is started.

### Acceptance Criteria
The above relationship model, and any future changes, should satisfy the following criteria:
1. Can assign a candidate to a panel
2. Can list all candidates in a panel
3. Identify which panel a candidate is in
4. Can list all candidates & the panels they are in
5. Can list all candidates which aren’t in a panel
6. Can support multiple types of panel (sift, selection)
7. Can support custom panel types (e.g. sift, selection, custom, custom2)