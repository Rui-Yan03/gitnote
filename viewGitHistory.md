## view the commit history

```
git log
```

-p: shows the difference introduced in each commit

--stat: show a list of modified files, how many files were changed, and how many lines in those file were added or deleted

--pretty=online: show commit history in a line

--pretty=format:"<someformat>"

## the difference between author and commiter

the author is who write the code and the committer is who applied the work to repo

--graph: display an ASCII graph of branch and merge history beside the log output

## limiting log output

--since: take a specific data like"2018-7-9" or relative date like "1 years 1 day 3 minutes ago"

--until

-S: take a string argument and show commits that only changed the occurrences of that string(you can check the change history of a function)

-- path/to/file: only show commits that introduce changed to that file

--no-merges

--before

--grep
