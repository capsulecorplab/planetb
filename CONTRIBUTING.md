# How to contribute

## Submitting features or changes

If you've been added as a collaborator, then clone project to your local machine:

```
git clone https://github.com/itsevalieu/planetb
```

Otherwise, fork the project (https://github.com/itsevalieu/planetb/fork), then clone the forked project to your local machine:

```
git clone https://github.com/<yourusername>/planetb
```

Checkout `develop` branch to create a new feature branch. Use the branch naming scheme, `issue<issue no>-feature-title`:

```
git checkout develop
git checkout -b issue42-add-logarithms
```

Use a present tense commit message, preferably one that's no more than 50 characters in length:

```
git commit -am "add logarithms"
```

Push new feature branch to origin:

```
git push origin issue42-add-logarithms
```

If you already have an in-progress feature branch in origin and your `develop` branch becomes out of date, fetch and rebase your working branch off `origin/develop`, then force push:

```
git fetch origin
git rebase origin/develop
git push origin issue42-add-logarithms --force
```

## Submitting a pull request (PR)

Note: we will be using the [ZenHub for GitHub](https://chrome.google.com/webstore/detail/zenhub-for-github/ogcgkffhplmphkaahpmffcafajaocjbd?hl=en-US) chrome extension.

1. Submit a PR, by setting your feature branch as `HEAD` and `develop` branch as `root`. 
2. Connect PR to its corresponding issue that it closes. 
3. Set ZenHub pipeline to "Review/QA"
4. Assign a reviewer.
5. When ready, add the `author ready` label to indicate that you are satisfied with the PR to be merged.

## Coming soon...

Continuous Integration (CI) will be setup to verify whether `develop` branch can be merged into `master` branch.