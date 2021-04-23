---
nav_exclude: true
---
# Top-level Overview

*** * * NOTE: This page is a work in progress * *  ***


## Entity-Relationship Diagram

![](top-level.svg)


## Collection: `exercises`

Documents in the `exercises` collection represent an exercise that will be undertaken by the Judicial Appointments Commission to
select and recommend candidates for a judicial role.

These documents are are created and maintained via the JAC Admin portal.


## Collection: `vacancies`

An exercise can be published by JAC staff via the Admin portal, at which point a copy of the `exercises` document is
created and stored in the `vacancies` collection.

Documents in the `vacancies` collection appear on the Apply website, which is open to the public: (i.e., potential candidates for the role).
Documents in the `exercises` collection only appear on the Admin portal.
This design is intended as a security measure: the master copy (from the `exercises` collection) can only be accessed from the Admin portal (i.e., by JAC staff).


## Collection: `applications`

Documents in the  `applications` collection represent a candidate's application for a judicial role.

These documents are created by candidates using the Apply website.


## Collection: `applicationRecords`
