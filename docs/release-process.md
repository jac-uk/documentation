# Release Process

We aim to release changes early and often so have a daily release cycle.

Every week day at midday we carry out the following steps:

## Finish the current release

Providing the current release has been reviewed and approved by the QA team we finish the release and deploy to production using the following commands 
    
```
git hf update
git hf release finish #version-number#
```

We provide a list of the issues in the release tag message using the following format
   
``` 
  #123 Add cancel button to sign up page
  #124 Add log out button to header
```

_Note: there's a single space at the start of each line so they're not regarded as comments (which start with #)._

When CircleCI has finished deploying the release to production we update the relevant issue in zenhub, ensuring each issue:
- [x] Has been tagged with the current sprint milestone
- [x] Has the correct version number label
- [x] Is moved to zenhub column "Released"

Finally we post release notes to Slack using the following format
```
@here the following changes have been released to production:

#Project# #Version#
- #123 Add cancel button to sign up page
- #124 Add log out button to header
```

## Start the next release

In zenhub we look at the "Ready for release" column to identify which issues are ready to be released.

We generate release notes in the following format
```
  #123 Add cancel button to sign up page
  #124 Add log out button to header
```
_Note the space at the start of each line_

To ensure we are up to date with the latest changes we run the following command
```
git hf update
```

We identify the version number of the next release by looking at the current version in `package.json` and then run the command
```
git hf release start #version-number#
```

When CircleCI has finished deploying the release to staging we update the relevant issues in zenhub, ensuring each issue:
- [x] Has been tagged with the current sprint milestone
- [x] Has the correct version number label
- [x] Is moved to zenhub column "Ready for review"

Finally we post release notes to Slack using the following format
```
@here the following changes have been released to staging and are ready for review:

#Project# #Version#
- #123 Add cancel button to sign up page
- #124 Add log out button to header
```

---

## Future refinement

The above process lends itself to refinement are considering options such as:

- Automate/script the above process as is
- Move away from the above command line model and perhaps have our CI tool hook into tag events (e.g v1.2.3-rc1 deploys to staging, v1.2.3 deploys to production)
- Replacing CircleCI with alternatives such as Github Actions and Google Cloud Build

