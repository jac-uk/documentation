---
nav_exclude: true
---
# Data Model: Panels

## Collection: Panels
A `Panels` document contains the following fields:
```
  exerciseId: String,
  name: String,
  type: String ('sift', 'selection'),
  members: [ { fullName: String, email: String, phone: String, title: String } ],
  dateFrom: Timestamp,
  dateTo: Timestamp,
  created: Timestamp,
  status: String ('draft', 'created', 'completed'),
  applicationsMap: { <applicationId> => { errors: Array, fileIds: Array } },
  drive: { driveId: String, folderId: String },
  members: [ { email: String, fullName: String, phone: String, title: String } ],
  processing: { current: String, queue: Array, errors: Array },
  status: String,
  statusLog: { approved: Timestamp, created: Timestamp, processing: Timestamp },
  type: String
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
