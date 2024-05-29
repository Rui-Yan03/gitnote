1. fork that project
2. git clone the fork repo
3. create a topic branch
4. make commits
5. push to that fork repo
6. make pull request

## sync with origin repo
```
git add remote upstream <url>
git fetch upstream
git checkout <topicBranch>
git merge upstream/main
git push origin <topicBranch>
```

## keep your Github public repository up-to-date
```
git checkout main
git pull <upstreamRepo>
git push origin main
```

or you can do this without type url everytime

```
git remote add <shortname> <url>
git fetch <shortname>
git branch --set-upstream-to=<shortname>/main main
git config --local remote.PushDefault origin
```

once above is done, the process become more simpler
```
git checkout main
git pull
git push
```