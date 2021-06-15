---
nav_order: 4
parent: Developer guide
---
# Hotfixes

## Frequency
Hotfixes should be made when there is a high urgency.

## Versioning

We use an adaptation of the Semantic Versioning Specification **MAJOR.MINOR.PATCH** adapted to our needs

**MAJOR** revision (new UI, lots of new features, conceptual change, etc.) - we don't change this very often

**MINOR** revision (maybe a change to a search box, 1 feature added, collection of bug fixes) - basically every daily release we increment this number

<strong>**PATCH** - bugfix - Whenever we do a hotfix, we increment this number between daily releases </strong>

# Hotfix Process

## 1. Make a branch

Find a tag branch where a bug is not present, (for example, previous release branch 0.15.0).

Check out this branch and make a hotfix branch based on the tag branch.

```
git checkout -b 'hotfix/#[ticket-number]-[keywords]'
```
eg. `git checkout -b 'hotfix/1321-fix-title-misspelling'`

---
## 2. Commit fixes
Make necessary changes, check locally, run linting and testing.
Commit and push to github.

---
## 3. Make a Pull Request
Create a PR on github for the branch you have made, requested changes are merged back onto the hotfix branch.

---
## 4. Finish the hotfix

When all changes are approved, merge the hotfix branch into `master` branch using the manual Action called ‘Deploy to Production’.
Also, merge hotfix branch into `main` branch.docs/developer-guide/release-process.md

![6](./images/release6.png)
---
