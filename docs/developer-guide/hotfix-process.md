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

To be updated

---
