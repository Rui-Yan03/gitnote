## remote-tracking branches

Remote-tracking branches are references to state of remote branches.

Remote-tracking braches are named as <remote>/<branch>.

## to update remote-tracking branches

```
git fetch <remote>
```

## pushing

1. to push same name remote branch `git push <remote> <branch>`

2. to push different name remote branch `git push <remote> <localbranch><remotebranch>`

when you do a fetch that bring new remote-tracking branches, you don't have local, editable copies of them. You can:

1. merge it to current branch `git merge <remote>/<branch>`
2. have a local branch to base it off that remote-tracking branch `git checkout -b <localbranch> <remote>/<branch>`

## tracking branches

Tracking branches are local branches that have a relationship to a remote brach so that when `git pull`, git automatically know which branch to merge.

1. to create a new tracking branch that have the same name of remote branch
```
git checkout --track <remote>/<branch>
```

more short hand

```
git checkout <branch>
```

2. to create a new branch that have a different name from remote branch

```
git checkout -b <branch> <remote>/<branch>
```

3. link a exsited branch to remote branch or to change track a remote branch
```
git branch -u <remote>/<branch> 
```

## check tracking status

```
git branch -vv
```

`git fetch --all`

## delete remote branch

```
git push <remote> --delete <branch>
```