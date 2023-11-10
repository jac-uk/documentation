---
nav_exclude: true
---
# Top-level Overview


## Entity-Relationship Diagram

![](top-level-platform.svg)


## Collection: `exercises`

Documents in this collection represent an exercise that will be undertaken by the Judicial Appointments
Commission to select and recommend candidates for a judicial role.

These documents are are created and maintained via the JAC Admin portal.


## Collection: `vacancies`

An exercise can be published by JAC staff via the Admin portal, at which point a copy of the `exercises` document is
created and stored in the `vacancies` collection.

Documents in the `vacancies` collection appear on the public Apply website, which is open to the public: (i.e.,
potential candidates for the role).
Documents in the `exercises` collection only appear on the Admin portal.
This design is intended as a security measure: the master copy (from the `exercises` collection) can only be accessed
from the Admin portal (i.e., by JAC staff).


## Collection: `applications`

Documents in this collection represent a candidate's application for a judicial role.

These documents are created by candidates using the public Apply website.


## Collection: `applicationRecords`

Documents in this collection are created in the Admin portal when the JAC start processing candidate applications.

These documents store extra information about candidate applications from the JAC point-of-view, for example:
whether character or eligibility issues have been flagged up for the candidate; whether an Equal Merit Provision
has been applied; whether reasonable adjustments should be applied.


## Collection: `candidates`

Documents this collection represent candidates applying for one or more judicial roles.


## Collection: `qualifyingTestReports`

Documents in this collection represent a report containing stastical data about one more qualifying tests,
such as: maximum test scores; individual test scores and rankings; diversity metrics.


## Collection: `assessments`

Documents in this collection represent an independant assessment of a candidate's application for a role.


## Collection: `panels`

Documents in this collection represent a review panel for an exercise.


## Collection: `invitations`

Documents in this collection represent an invitation for a candidate to apply for a judical role.

JAC can send invitations from the Admin portal.


## Collection: `notifications`

Documents in this collection represent notifications that have been sent by the system, for example:
- A invite/reminder to an applicant about a qualifying test
- A request to an independent asseesors, to assess an application


## Collection: `notes`

Documents in this collection contain notes about a candidate.


## Collection: `logs`

Documents in this collection represent a log of an event in the system, for example:
- information log
- warning log
- error log
- user login

Event logs can be viewed from within the JAC Admin portal.


## Collection: `meta`

Documents in this collection contain general statistics about the system, for example: the number of exercises
in the system.


## Collection: `settings`

Documents in this collection contain various system settings.
