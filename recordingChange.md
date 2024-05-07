## 2 kinds file
1. untracked file: not in last snapshot and not in staging area
2. tracked file: anything else.

## check status

```
git status
```

## tracking new file

```
git add <file/dire>
```
when staged file is changed, save changes to staged area

```
git add <file>
```

## short status

```
git status -s
```

??: new file not tracked
M: modified
A: new files that have been added to staging area

lefthand column indicates the staging area and righthand the working tree

## ingnoring file
to make git not remind sth untracked, add them to .gitignore

1. standard glob patterns work, and will work recursively
2. start pattern with / to avoid recursive
3. end pattern with / to specify a directory
4. negate a pattern(do not ignore) by add ! in front of pattern
**: match nested dire

/todo
to ingore todo in current dire not sub/todo

todo/
to ingote all file under todo

!lib.a
not ingore lib.a

## view your staged and unstaged changes
1. to see what have changed but not staged(compare working directory and staging area)

```
git diff
```

2. to see what you've staged will go into next commit(compare staging area and last commit)

```
git diff --staged/cached
```


## skipping the staging area
-a flag will stage all changed files


## removing files

1. remove working directory file

```
rm file.txt
git rm file.txt
```

2. remove staged file

```
git rm --cached file.txt
```


