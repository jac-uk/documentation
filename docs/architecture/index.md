---
title: Architecture
nav_order: 2
has_children: true
---
# JAC Digital Platform

The JAC Digital Platform is hosted in [Firebase](https://firebase.google.com) (part of [Google Cloud](https://cloud.google.com)) which provides cloud-based services such as authentication, database, storage, hosting and functions.

Our 'front end' apps are lightweight [Single Page Applications (SPAs)](https://en.wikipedia.org/wiki/Single-page_application) using [Vue.js](https://vuejs.org). They connect to firebase services using the [Firebase SDK](https://firebase.google.com/docs/reference/js).

We use [Firestore](https://firebase.google.com/docs/firestore) as our primary cloud-based database. [Firestore Security Rules](https://firebase.google.com/docs/firestore/security/get-started) enable us to specify granular access to data and [Indexes](https://firebase.google.com/docs/firestore/query-data/index-overview) enable us to efficiently query our data.

We use [Cloud Storage](https://firebase.google.com/docs/storage) to store and serve files. [Storage Security Rules](https://firebase.google.com/docs/storage/security/start) enable us to specify granular access.

We use [Cloud Functions](https://firebase.google.com/docs/functions/) to execute 'back end' code in response to defined triggers.

We are starting to use services from the wider Google Cloud such as [BigQuery](https://cloud.google.com/bigquery) for custom reports and [AppEngine](https://cloud.google.com/appengine) for our API.