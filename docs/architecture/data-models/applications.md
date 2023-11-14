# Data Model: Applications

This document outlines the structure of the `applications` collection.

## Collection: Applications

A `applications` document contains the following fields:

| Field                                                     | Type      | Description                                              |
| --------------------------------------------------------- | --------- | -------------------------------------------------------- |
| experience                                                | array     | Post-qualification experience                            |
| experience.jobTitle                                       | string    | Job title                                                |
| experience.orgBusinessName                                | string    | Name of the organization or business                     |
| experience.startDate                                      | timestamp | Start date                                               |
| experience.endDate                                        | timestamp | End date                                                 |
| experience.isOngoing                                      | boolean   | Indicates if the experience is ongoing                   |
| experience.tasks                                          | array     | Law-related tasks within this role                       |
| experience.judicialFunctions                              | map       | Involvement in judicial functions of courts or tribunals |
| experience.judicialFunctions.type                         | string    | Type of judicial or quasi-judicial post                  |
| experience.judicialFunctions.duration                     | number    | Accumulated sitting days in this post                    |
| experience.judicialFunctions.isLegalQualificationRequired | boolean   | Requirement of legal qualification for appointment       |
| experience.judicialFunctions.details                      | string    | Overview of powers, procedures, and responsibilities     |
| experience.taskDetails                                    | map       | Specific task details                                    |
| experience.taskDetails.jurisdiction                       | string    | Primary operating location or region                     |
| experience.taskDetails.location                           | string    | Jurisdiction or area of law                              |
| experience.taskDetails.workingBasis                       | string    | Basis of work                                            |
| experienceDetails                                         | string    | Details of how you have acquired the necessary skills    |
| employmentGaps                                            | array     | Employment gaps                                          |
| employmentGaps.details                                    | string    | Details of the employment gap                            |
| employmentGaps.startDate                                  | timestamp | Start date                                               |
| employmentGaps.endDate                                    | timestamp | End date                                                 |
| employmentGaps.isOngoing                                  | boolean   | Indicates if the employment gap is ongoing               |
| employmentGaps.tasks                                      | array     | Law-related tasks within this role                       |

## Application Version 3

Version 3 of the application introduces additional fields within the `experience` section:

| Field                                                     | Type      | Description                                              |
| --------------------------------------------------------- | --------- | -------------------------------------------------------- |
| experience.isOngoing                                      | boolean   | Indicates if the experience is ongoing                   |
| experience.judicialFunctions                              | map       | Involvement in judicial functions of courts or tribunals |
| experience.judicialFunctions.type                         | string    | Type of judicial or quasi-judicial post                  |
| experience.judicialFunctions.duration                     | number    | Accumulated sitting days in this post                    |
| experience.judicialFunctions.isLegalQualificationRequired | boolean   | Requirement of legal qualification for appointment       |
| experience.judicialFunctions.details                      | string    | Overview of powers, procedures, and responsibilities     |
| experienceDetails                                         | string    | Details of how you have acquired the necessary skills    |
