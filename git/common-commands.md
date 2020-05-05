# Git cheat sheet

Please read our [getting started](setup.md) instructions.

#### Stay up to date
Do this at least once a day
```
git hf update
```

### Start working on a new feature
```
git hf feature start ##feature-name##
```

### Start working on an existing feature
```
git hf feature checkout ##feature-name##
```


#### Push your work to github
Do this regularly so others can see what you’re working on and there’s a backup
```
git hf push
```

#### Pull changes from github
If you’re collaborating on a feature with other developers, make sure you have their changes too
```
git hf pull
```


#### Finish working on a feature
Use GitHub website to create a Pull Request and ask (assign) a colleague to review

Once approved (and then merged) the feature can be closed

```
git hf feature finish
```



#### Naming features

Use kebab-case and name your feature with a reference number from GitHub. Choose the reference number of the primary issue you are working on.

e.g. a fictional feature might be `123-add-reset-button`



<!-- Release

Create a release branch
git hf update
git hf release start ##version-number##

Remember to increment the version number in code accordingly

Test and fix until the release is ready

Finish the release
git hf release finish ##version-number##


Hot Fix

Create a new hotfix
git hf update
git hf hotfix start ##version-number##
Finish a hotfix
git hf hotfix finish ##version-number## -->

