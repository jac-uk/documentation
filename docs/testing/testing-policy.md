---
nav_order: 1
parent: Testing
---
# Testing policy

The JAC aims to test early, often and throughout the discovery, design and build of our services.

No changes are allowed to our services unless they pass various automated and manual tests.

Our current (Sep 2021) testing steps for all changes (new features, improvements and fixes) are outlined below.

Developers run unit tests and lint checks in their local development environments before changes are pushed to our code repository.

All changes are pushed to new branches and are not allowed in our main code base until they have passed a number of checks:

* Automated unit tests and lint checks are run along with automated code scanning to check for security vulnerabilities and coding errors.
* Changes are manually code reviewed by multiple developers.
* Changes are automatically deployed to preview URLs and manually tested by the product team and at least two user representatives (via the User Testing Group). Developers create short videos to demonstrate how functionality should work and place them into a Google drive [folder](https://drive.google.com/drive/folders/1-kkQ1_ArvpIiHIid7NBPDzwnPoss0TPR).
Links to the description of functionality and preview URLs are posted to the 'user-testing' channel on Slack. Business Analyst and members of the User Testing Group review videos and [test scripts](https://drive.google.com/drive/u/0/folders/142leRfwBIMZQbmZXivGzhcYrYTUfYUOS), test the functionality and post results into the Slack channel.

When all checks have passed the approved changes are merged into our main codebase and automatically deployed to our staging (pre-production) environment.

On staging the changes are manually verified and staging is also checked for regressions.

When all is ok the change will be released to production.
