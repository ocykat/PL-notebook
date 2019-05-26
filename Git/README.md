# Git

## Submodules

### Cloning submodules
To clone a child repo to the current repo:

```sh
# clone
git submodule add <url of child repo>
# initialize submodule configuration
git submodule init
```

If you want to specify the master branch to be the branch to track:

```sh
git submodule add -b master <url to child repo>
```

### Getting updates of submodules
To get updates from the submodule:
```sh
git submodule update --remote
```