## create a new branch
```
git branch <branch>
```

## switch to a branch
```
git checkout <branch>
```

## create a new branch and swithing to it
```
git checkout -b <branch>
```
or 
```
git switch -c <branch>
```

## show where the branch pointers are pointing
```
git log --oneline --decorate
```

## `git log` doesn't show all branches all time, it only show commit history blow the branch you've checked out.
1. to show commit history of desired branch
```
git log <branch>
```

2. to show all branches
```
git log --all
```
