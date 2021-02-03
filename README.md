# How to git

## Starting

To clone a project:

```
git clone https://github.com/USER/REPO.git
```

If you have created a local directory, go inside and do

```
git init
git remote add origin https://github.com/USER/REPO.git
git push origin master
```

## Updating local information
```
git fetch
```

## About branches

To list branches (after you fetch)
```
git branch -a
```

To create a new branch
```
git checkout -b new_branch
```

To get a branch
```
git checkout branch
```

## Changes and updating
On making and saving your changes
```
git add file
git commit -m "A comment"
git push origin branch
```

On updating from remote
```
git pull origin branch
```

## Merging between branches
```
git checkout branch1
git merge branch2 # branch2 changes go into branch1
git push origin branch1
```

## Stashing
If you forgot to update your local repo, and you have made changes you might get conflicts.  You can stash your changes, update and then unstash

```
git stash
git pull origin branch
git stash apply
```
## Removing
To remove files or diretory do
```
git rm file
git rm -r dir
``
Then commit and push. 

If you want to delete something from the repo but not locally, add the flag `--cached` to `git rm`



