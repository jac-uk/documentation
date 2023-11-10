---
nav_exclude: true
---
# Data Model: applications

## Collection: applications
A `applications` document contains the following fields:

| Field                                                     | Type      | Description                                                   |
| --------------------------------------------------------- | --------- | ------------------------------------------------------------- |
| experience                                                | array     | Post-qualification experience                                 |
| experience.jobTitle                                       | string    | Job title                                                     |
| experience.orgBusinessName                                | string    | Organisation or business name                                 |
| experience.startDate                                      | timestamp | Start date                                                    |
| experience.endDate                                        | timestamp | End date                                                      |
| experience.tasks                                          | array     | Law-related tasks in this role                                |
| experience.taskDetails                                    | map       | The task details                                              |
| experience.taskDetails.jurisdiction                       | string    | Base location and/or region where you predominately operate/d |
| experience.taskDetails.location                           | string    | Jurisdiction/area of law                                      |
| experience.taskDetails.workingBasis                       | string    | Working Basis                                                 |



## Application Version 3

The following fields have been added to the post-qualification experience in the application version 3:

| Field                                                     | Type      | Description                                                     |
| --------------------------------------------------------- | --------- | --------------------------------------------------------------- |
| experience.isOngoing                                      | boolean   | Still ongoing                                                   |
| experience.judicialFunctions                              | object    | The carrying-out of judicial functions of any court or tribunal |
| experience.judicialFunctions.type                         | string    | Is this a judicial or quasi-judicial post?                      |
| experience.judicialFunctions.duration                     | number    | How many sitting days have you accumulated in this post?        |
| experience.judicialFunctions.isLegalQualificationRequired | boolean   | Is a legal qualification a requisite for appointment?           |
| experience.judicialFunctions.details                      | string    | Outline the powers, procedures and main responsibilities        |
