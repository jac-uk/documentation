# Panels Data Model

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
    sift: String,
    selection: String,
  }
```
Each `type` of panel will have an entry in the `panelIds` map. These entries will be initialised to an empty string (to indicate the application has not been assigned to a panel) and eventually assigned the `id` of a `Panels` document.
Initialising the `panelIds` map will happen when the respective panel task is started.