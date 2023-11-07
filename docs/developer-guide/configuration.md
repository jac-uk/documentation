---
nav_order: 6
parent: Developer guide
---

# Configuration

Configuration values can be set based upon each application and environment it's needed for.

## QT

The QT platform is split into 3 applications: QT-Admin, QT and Platform.

Each of these apps has its own dedicated .env files for each environment.

## Admin/Apply/Assessments

All of these apps have their own dedicated .env files for each environment.

## Digital Platform

When working in nodeScripts you can use the .env file (see nodeScripts/shared/config.js) to set configuration variables.

However when you want to set configuration variables outside the nodeScripts you have to do the following:

### Local Environment
Store the values in your .runtimeconfig.json file and reference them in the config.js files (eg see: functions/shared/config.js)

>.runtimeConfig

`{
  "tester": {
    "test_url": "https://www.google.com/test",
  },
}`

>functions/shared/config.js

`module.exports = {
  GOOGLE_TEST_URL: functions.config().tester.test_url,
}`

### Develop/Staging/Production
Examples of getting and setting config variables
> firebase functions:config:get
> firebase functions:config:set zenhub.graph_ql_url=https://api.zenhub.com/public/graphql

---
