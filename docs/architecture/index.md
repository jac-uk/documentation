# Architecture

We are loosely following the [C4 Model](https://c4model.com) for diagramming our software architecture.

## Level 1: System Context diagram

The following context diagram is suitable for anyone to gain a high-level overview of the system. It shows the main personas interacting with the Digital Platform and the existing software systems it connects to.

![System Context diagram](jac-overview-Context.svg)]


## <a name="container"></a> Level 2: Container diagram

The following diagram is aimed at support and operations staff as well as developers and architects. It shows the primary "containers" that comprise the Digital Platform, which are:

- Admin - a single page application aimed at enabling JAC staff to create and manage exercises and the applications received to those exercises
- Apply - a single page application aimed at enabling candidates to view vacancies, check their eligibility, apply and monitor their application
- Assessments - a single page application aimed at enabling assessors (eseentially candidate referees) to provide an independent assessment (reference) for a candidate
- Cloud Firestore - is a cloud-based database within which we store exercise, candidate, application, assessor and related data
- Firebase Authentication - is a cloud-based authentication service used to identify our users and ensure they have appropriate access
- Cloud Storage - is a cloud-based file storage service whene we store all candidate and assessor files
- Cloud Functions - are cloud-based pieces of functionality that can be run in response to defined triggers (e.g. when a candidate applies for an exercise), scheduled to run in the background (e.g. automatic backups) or called directly (e.g. send a batch of emails)


[![Container diagram](jac-overview-Container.svg)](#component)

## Level 3: Component diagrams

The following diagrams are aimed at architects and developers and show more detail on the components of the software containers we are developing. In particular we identify the key configurables of each container.

_Coming soon!_


## Level 4: Code diagrams

We do not currently have any code diagrams. As a small agile team it is unlikely we will add any anytime soon.
