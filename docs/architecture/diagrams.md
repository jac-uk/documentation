---
nav_order: 2
parent: Architecture
title: Diagrams
---

# Architecture Diagrams

We are loosely following the [C4 Model](https://c4model.com) for diagramming our software architecture.
We use [diagrams.net](https://www.diagrams.net) to create and edit our diagrams.

## <a name="context"></a> Level 1: System Context diagram

The following context diagram is suitable for anyone to gain a high-level overview of the system. It shows the main personas interacting with the Digital Platform and the existing software the system connects to.

![System Context diagram](jac-overview-Context.svg)


## <a name="container"></a> Level 2: Container diagram

The following diagram is aimed at support and operations staff as well as developers and architects. It shows the primary "containers" that comprise the Digital Platform.

![Container diagram](jac-overview-Container.svg)

We have three user-facing containers. All are [Single Page Applications (SPAs)](https://en.wikipedia.org/wiki/Single-page_application) using [Vue.js](https://vuejs.org). They are hosted in [Firebase Hosting](https://firebase.google.com/docs/hosting) and connect to our cloud back end services using the [Firebase SDK](https://firebase.google.com/docs/reference/js).

**Admin** is a single page application aimed at enabling JAC staff to create and manage exercises and the applications received to those exercises.

**Apply** is a single page application aimed at enabling candidates to view vacancies, check their eligibility, apply and monitor their application.

**Assessments** is a single page application aimed at enabling assessors (essentially referees) to provide an independent assessment (reference) for a candidate.

Our cloud back end services are all based in [Firebase](https://firebase.google.com).

**[Cloud Firestore](https://firebase.google.com/docs/firestore)** is a cloud-based database within which we store exercise, candidate, application, assessor and related data.

**[Firebase Authentication](https://firebase.google.com/docs/auth)** is a cloud-based authentication service used to identify our users so we can ensure they have appropriate access.

**[Cloud Storage](https://firebase.google.com/docs/storage)** is a cloud-based file storage service where we store all candidate and assessor files.

**[Cloud Functions](https://firebase.google.com/docs/functions/)** are cloud-based pieces of functionality that can be run in response to defined events (e.g. when a candidate applies for an exercise), scheduled (e.g. automatic backups) or called directly (e.g. send a batch of emails).


## <a name="component"></a> Level 3: Component diagrams

The following diagrams are aimed at architects and developers and show more detail on the components of the software containers being developed. In particular we identify the key configurables of each cloud-based container.

Our functions are grouped as follows:

- **Background Functions** are automatically triggered when defined events happen, for example when a candidate applies for a vacancy
- **Callable Functions** are primarily triggered from our 'front end' apps, for example when a user wishes to send a batch of emails.
- **Scheduled Functions** are triggered according to a pre-defined schedule, for example backups are made on an hourly basis.

**[Apply. Character Information](character-information.md)**


## Level 4: Code diagrams

As a small agile team it is unlikely we will add many code diagrams anytime soon.
