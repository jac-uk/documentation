---
nav_exclude: true
---
# Eligibility issues

## Version 2
Used in legal exercises from June 2024. Is for user can add recommendation and comment for each eligibility issue. The recommendations, comments and related data are saved in following fields:
- issue type: `applicationRecords.issues.eligibilityIssues[].type`
- JAC comments: `applicationRecords.issues.eligibilityIssues[].comments`
- recommendation: `applicationRecords.issues.eligibilityIssues[].result`
- candidate comments: `applicationRecords.issues.eligibilityIssues[].candidateComments`
- met or not met: `applicationRecords.issues.eligibilityIssues[].summary`
- SCC age: `applicationRecords.issues.eligibilityIssues[].sccAge` (only if type = 'rls' which is reasonable length of service has this field)

## Version 1
Only used in non legal exercises, user can add one overall recommendation and comment for all the eligibility issues. In June 2024 legal exercises migrate to V2 by `nodeScripts/updateApplicationRecordEligibilityIssueToVersion2.js`.

The recommendation and comment will save in following fields:
- JAC comments: `applicationRecords.eligibilityIssuesStatusReason`
- recommendation: `applicationRecords.eligibilityIssuesStatus`