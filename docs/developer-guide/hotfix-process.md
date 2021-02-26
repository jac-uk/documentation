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
## 1. Start the hotfix
First ensure you have latest code.

```
git hf update
```
then start a hotfix branch
```
git hf hotfix start [VERSION]
```
bump the patch number in `package.json`

---
## *Important*
### Any changes pushed to a 'hotfix/...' branch will deploy to production.
### If you make any commits, dont push them to the remote branch

---

## 2. Make a branch

Make a branch off of the hotfix branch you have created

```
git checkout -b 'bug/#[ticket-number]-[keywords]'
```
eg. `git checkout -b 'bug/#123-remove-bug'`

---
## 3. Commit fixes
Make necessary changes, check locally, run linting and testing.
Commit and push to github.

---
## 4. Make a Pull Request
Create a PR on github for the branch you have made, requested changes are merged back onto the hotfix branch.

---
## 5. Finish the hotfix

Pushes made to a hotfix instantly begin the process of being deployed to production.

When finished, these changes will also be deployed to develop.

Changes WILL NOT be deployed to staging until the next release.

If there is currently a release branch, rebasing said release branch off of the updated develop branch, following a hotfix, will ensure changes reach staging.

Make sure you are aware of any updates to other branches which could cause merge conflicts.

After the PR has passed review, get the latest code
```
git hf update
```
and switch to the hotfix branch
```
git checkout 'hotfix/[VERSION]'
```
then finish the hotfix with
```
git hf hotfix finish [VERSION]
```
---
