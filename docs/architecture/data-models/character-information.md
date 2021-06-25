---
nav_exclude: true
---
# Data Model: Exercise and Vacancy

A new field `_applicationVersion` was added to these data models to enable support for both old and new versions of the application form.

# Data Model: Application

The data entered into the new applications is stored in `characterInformationV2` and for old applications it is stored in `characterInformation`.

# Data Model: Candidate

The data is stored in `documents/characterInformation` for both old and new applications and a new field `_versionNumber` was added to this model. 
