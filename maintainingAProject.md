## if the merge is trivial
hit the merge button on the Github site.

## pull the code down and merge locally
to test
```
git checkout -b <testBranch> main
git pull <pullrequest>
```

```
git checkout main
git merge <testBranch>
git push origin main
```

## if you manage many pullrequests
1. fetch a particular pr
get list of prs
```
git ls-remote <remote>
```

fetch particular into FETCH_HEAD, then you can merge FETCH_HEAD into the branch you want to merge.
```
git fetch <lsitem>
```

2. fetch all prs
go to .git/config to append code under [remote "origin"] item
```
[remote "origin"]
    fetch = +refs/pull/*/head:refs/remotes/origin/pr/*
```

then you can fetch all prs
```
git fetch
```

then you can checkout pr
```
git checkout <pr>
```