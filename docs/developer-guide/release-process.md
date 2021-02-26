---
nav_order: 3
parent: Developer guide
---

# Deployment

## Frequency
We aim to release changes early and often so have a daily release cycle that starts and ends at midday.


## Versioning
We use an adaptation of the Semantic Versioning Specification **MAJOR.MINOR.PATCH** adapted to our needs


**MAJOR** revision (new UI, lots of new features, conceptual change, etc.) - we don't change this very often

**MINOR** revision (maybe a change to a search box, 1 feature added, collection of bug fixes) - basically every daily release we increment this number

**PATCH** - bugfix - Whenever we do a hotfix, we increment this number between daily releases


## Release Process
Every week day at midday we carry out the following steps:

## 1. Finish the current release

Check zenhub

Providing the current release has been reviewed and approved by the QA team we finish the release and deploy to production using the following commands

```
git hf update
git hf release finish [VERSION]
```
We provide a list of the issues in the release tag message using the following format

```
 #123 Add cancel button to sign up page
 #124 Add log out button to header
```

_Note: there's a single space at the start of each line so they're not regarded as comments (which start with #)._

When CircleCI (https://app.circleci.com/pipelines/github/jac-uk) has finished deploying the release to production we update the relevant issues in zenhub ensuring each one:
- [x] Has been tagged with the current sprint milestone
- [x] Has the correct version number label
- [x] Is moved to zenhub column "Released"

Post these release notes to Slack channel **#digital-team** using the following format:

> @channel version **[VERSION]** has been released to **[APP]** production
> 2 issues / 16.5 sp
>
> https://**[APP]**.judicialappointments.digital/
>
> * #123 Add cancel button to sign up page
> * #124 Add log out button to header

Finally add the same message to the respective apply/admin section of the release notes email.

## 2. Start the next release

In zenhub (https://app.zenhub.com/workspaces/platform-development-5ea838cd2aec471eb6d14139/board) we look at the "Ready for release" column to identify which issues are ready to be released.

We generate release notes in the following format
```
 #123 Add cancel button to sign up page
 #124 Add log out button to header
```

- Add these notes to the local `release-notes.md` file in each repo

_Note the space at the start of each line_

To ensure we are up to date with the latest changes we run the following command
```
git hf update
```

We identify the version number of the next release by looking at the current version in `package.json` and then run the command
```
git hf release start [VERSION]
```
Then update `package.json` version to match.

When CircleCI (https://app.circleci.com/pipelines/github/jac-uk) has finished deploying the release to staging we update the relevant issues in zenhub ensuring each one:
- [x] Has been tagged with the current sprint milestone
- [x] Has the correct version number label ("**[APP]**: **[VERSION]**" in `#ff9933`, labels have to be created in the relevant repository if they don't exist)
- [x] Is moved to zenhub column "Ready for review"


Finally we post release notes to Slack channel **#digital-team** using the following format:

> @channel version **[VERSION]** has been released to **[APP]** staging and following changes are ready for review:
> 2 issues / 16.5 sp
>
> https://**[APP]**-staging.judicialappointments.digital/
>
> * #123 Add cancel button to sign up page
> * #124 Add log out button to header

---

## Future refinement

The above process lends itself to refinement and we are considering options such as:

- Automate/script the above process as is
- Move away from the above command line model and perhaps have our CI tool hook into tag events (e.g v1.2.3-rc1 deploys to staging, v1.2.3 deploys to production)
- Replacing CircleCI with alternatives such as Github Actions and Google Cloud Build

