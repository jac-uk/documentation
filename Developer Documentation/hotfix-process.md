# Hotfixes

## Frequency
Hotfixes should be made when there is a high urgency. 

## Versioning
We use an adaptation of the Semantic Versioning Specification **MAJOR.MINOR.PATCH** adapted to our needs

**MAJOR** revision (new UI, lots of new features, conceptual change, etc.) - we don't change this very often

**MINOR** revision (maybe a change to a search box, 1 feature added, collection of bug fixes) - basically every daily release we increment this number

<strong>**PATCH** - bugfix - Whenever we do a hotfix, we increment this number between daily releases </strong>

# Hotfix Process
## 1. Start the next release
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

## 2. Commit fixes
Make necessary changes, check locally, run linting and testing.

## 3. Make a PR branch
** *update on first use* **

Make a branch off of the hotfix branch
```
git checkout -b 'hotfix/[VERSION]'
```
commit, push to github and create a PR

## 4. Finish the hotfix

After the PR has passed reviewed, finish the hotfix
```
git hf hotfix finish [VERSION]
```
---