---
nav_exclude: true
---
# Top-level Overview

*** * * NOTE: This page is a work in progress * *  ***


## Entity-Relationship Diagram

![](top-level.svg)


## Collection: `exercises`

The `exercises` collection represents an exercise that will be undertaken by the Judicial Appointments Commission to
select candidates for a judicial role.

Documents in this collection are created and maintained via the JAC _Admin_ portal.


## Collection: `vacancies`

An exercise can be published by JAC staff via the _Admin_ portal, at which point a copy of the `exercise` document is
created and stored in the `vacancies` collection.
Documents in the `vacancies` collection appear on the _Apply_ website, which is open to the public (i.e., potential candidates).
Documents in the `exercises` collection only appear on the _Admin portal.
This design is intended as a security measure: the master copy (from the `exercises` collection) can only be accessed by JAC staff.


## Collection: `applications`

This collection represents a candidate's application for a judicial role.
Documents in this collection are created by candidates using the _Apply_ website.


## Collection: `applicationRecords`
