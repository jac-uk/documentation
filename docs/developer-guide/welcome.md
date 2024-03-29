---
nav_order: 1
parent: Developer guide
title: Welcome
---

# Welcome to JAC Digital

![JAC values](images/jac-values.png)

## Tools we use

We make use of the following tools:
- Github Issues for tracking and managing tasks
- Zenhub for managing Github Issues
- Github Actions for continuous integration and deployment, releases and hotfixes
- Github Flow model for organising our source code

Here is a more detailed list of all [software used and owners](https://drive.google.com/drive/folders/1R7XF1fecakMDNR7ZIftSlnu0F5NbUwh7)

## Our standards

We follow these [software development standards and guidelines.](https://docs.google.com/document/d/1nf4zyu-QTZmwqNylOQjZq2dTVeVSQBRlZNj3uEyerRc)

## Permissions

New starters will be assigned the following permissions

### Firebase

**Digital Staff** will be assigned the following Roles:

- Platform - Develop: `Firebase Admin`
- Platform - Staging: `Firebase Viewer`
- Platform - Production: `Firebase Viewer`

**Digital Suppliers** will be assigned the following Roles:

- Platform - Develop: `Firebase Admin`
- Platform - Staging: `Firebase Viewer`

### Github

**Digital Staff** will be added to `JAC Staff Team` which gives write or owner access to all repositories

**Digital Suppliers** will be added to `Digital Suppliers` team which gives write access to our six main repositories

### GovUK Notify

We have the following three api keys for GovUK Notify:

- `Digital Platform - Live`  sends emails to anyone
- `Digital Platform - Limited`  sends emails to JAC users (of GovUK Notify) only
- `Digital Platform - Test`  does not send emails

These should be used as follows:

- Production uses `Digital Platform - Live`
- Staging uses `Digital Platform - Test`
- Develop uses `Digital Platform - Test`

Developers may temporarily use `Digital Platform - Limited` on develop or staging however must change back to using `Digital Platform - Test`

Keys are stored in `firebase functions:config` and also may temporarily be stored locally in `.env`
