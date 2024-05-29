## the basic rebase

```
git checkout <rebaseBranch>
git rebase <branchToBeBasedOn>
git checkout <branchToBeBasedOn>
git merge <rebaseBranch>
```

## rebase branches who have same parent

```
git rebase <branchToBeBasedOn> <rebaseBranch>
git checkout <branchToBeBasedOn>
git merge <rebaseBranch>
```
## rebase branches who not have same parent

```
git rebase --onto <brachToBeRebasedOn> <brachDivergedFrom> <divergedBranch>
```

rebase commits that diverged from <brachDivergedFrom> in <divergedBranch> onto <branchToBeRebaseOn>

## note!

You can get the best of both worlds: rebase local changes before pushing to clean up your work, but never rebase anything that you’ve pushed somewhere.