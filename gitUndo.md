## undo things
when you forget add some after commit and you want to add that files to make 1 commit not 2, use --amend

```
git commit -m "Initial commit"
git add some.file
git commit --amend
```
will end up with a single commit, the second will replace the first one

## unstaging a staged file

```
git restore --staged <file>
```

## unmodifying a modified file
to revert a file back to what it like in last commit

```
git restore <file>
```
## revert file in state of previous commit

```
git checkout <hash> -- <file>
```
