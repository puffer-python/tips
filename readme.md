Welcome, you guys, to contribute your tips to everyone by creating a pull request [![GitHub issues](https://img.shields.io/github/issues/puffer-python/tips)](https://github.com/puffer-python/tips/issues)
## Linux
### RUN cmds in a file 

```cmd
while read p; do   bash -c  "$p"; done < tet.ok
```
## GIT
### Delete all local branches except a branch

```cmd
git branch | grep -v "master" | grep -v "branch_1" | xargs git branch -D
```
