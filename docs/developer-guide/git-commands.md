# Git commands


## Getting started

We currently follow the [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/) model and are using [Hub Flow](https://datasift.github.io/gitflow/TheHubFlowTools.html) extensions to assist with this. 


Install Hub Flow as follows
```
git clone https://github.com/datasift/gitflow
cd gitflow
sudo ./install.sh
```

Clone the repo you are working on and initialise Hub Flow, for example
```
git clone https://github.com/jac-uk/apply.git
cd apply
git hf init
```

Stay up to date with the repository you are working on by running the following command regularly

```
git hf update
```


## Working on features


Start working on a new feature
```
git hf feature start ##feature-name##
```

Start working on an existing feature
```
git hf feature checkout ##feature-name##
```

Push your work to github
```
git hf push
```

Pull changes from github
```
git hf pull
```

When you want to finish working on a feature use github website to create a Pull Request and ask for approval. When it has been approved and merged the feature can be finished (closed)
```
git hf feature finish
```


Tips:
- Push your code regularly so others can see what you're working on and there’s a backup
- When collaborating on a feature pull changes regularly



#### Naming features

Use [kebab-case](https://en.wiktionary.org/wiki/kebab_case#English) and name your feature with a reference number from GitHub. Choose the reference number of the primary issue you are working on.

e.g. a fictional feature might be `123-add-reset-button`



## Releases

Release branches are based off of `develop` and are deployed to staging.

Start a release branch
```
git hf update
git hf release start ##version-number##
```

Increment the version number in `package.json` accordingly then test and fix until the release is ready

Finishing the release will result in the changes being deployed to production and merged into `master` (and `develop`)
```
git hf release finish ##version-number##
```

## Hot fixes

Hotfix branches are based off of `master` and deployed straight to production

Start a new hotfix branch
```
git hf update
git hf hotfix start ##version-number##
```

Increment the version number in `package.json` accordingly

Finish the hotfix will result in the changes being merged into `master` and `develop`
```
git hf hotfix finish ##version-number##
```
