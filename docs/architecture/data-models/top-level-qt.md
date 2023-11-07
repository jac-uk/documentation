---
nav_exclude: true
---
# Top-level Overview


## Entity-Relationship Diagram

![](top-level-qt.svg)


## Collection: `qualifyingTests`

Documents this collection represent online tests which candidates applying for a judicial role must sit.

Note: Not all exercises/vacancies have qualifying tests.
Note: Equal Merit Tie-breaker tests are also stored in the `qualifyingTests` collection, denoted by the
`isTieBreaker` flag on the document.


## Collection: `qualifyingTestResponses`

After an online test has been created for an exercise the JAC selects candidates that should sit the test.
The test is then _activated_ by the JAC, at which point a copies of the test are created in the `qualifyingTestResponses`
collection for each candidate. These documents are start off as blank test papers, and eventually store
candidate's answers (responses).


## Collection: `logs`

Documents in this collection represent a log of an event in the system, for example:
- information log
- warning log
- error log
- user login

Event logs can be viewed from within the JAC Admin portal.


## Collection: `folders`

Documents in this collection contain folder names.


## Collection: `settings`

Documents in this collection contain various system settings.
