##show tags
1. list tags
```
git tag
```

2. show matched tags
``
git -l <partten>
```

3. show a specific tag information
```
git show <tagname>

##2 kinds of tag
1. lightweight tag
It's basically the commit checksum stored in a file.

To create a lightweight tag
```
git tag <tagname>

2. annotated tag
Annotated tag is store as full objects in Git database including tagging message.

To created a annotated tag
```
git tag -a <tagname> -m <message>
```

##creating tags later
```
git tag <tagname> <commithash>
git tag -a <tagname> <commithash>
```

##sharing tags
By default, `git push` doesn't transfer tags to remote server.You have to explicitly push tags to remote server.

1. push a specific tag
```
git push <remote> <tag>
```

2. push all annotated tags
```
git push <remote> --follow-tags

3. push all lightweight and annotated tags
```
git push <remote> --tags
```

##deleting tags
1. delete on local repo
```
git tag -d <tag>
```

2. push deleted tag to remote sever
```
git push <remote> :refs/tags/<tag>
```
or
```
git push <remote> --delete <tag>
```

## checking out tag
```
git checkout <tag>
```

And now, you are in "detached HEAD" state.If you make a commit, this commit will be unreachable and belong no branch, except exact commit hash.So when you want to commit create a branch.
```
git branch -b <branchname> <tag>
```

