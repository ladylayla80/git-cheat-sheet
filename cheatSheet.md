# Git cheat sheet

## Create
Clone existing github repository:

```
git clone https://github.com/USERNAME/GITREPONAME.git
```

Create new local repository:

```
git init
```

## Local changes
See changes in working directory:

```
git status
```
or

```
git diff
```

See changes made to file:

```
git diff <file>
```

Add all current changes to commit:

```
git add -A
```
or

```
git add .
```

Add specific file:

```
git add -p <file>
```

Commit all previously added changes:

> This way vim will open and you can type more detailed description

```
git commit
```
or

> This way you can type smaller description

```
git commit -m "COMMENT"
```

Get back to last commit:

```
git commit -a -amend
```

## Commit history and logs

Show commit history in single lines:

```
git log --oneline
```

Show commit history for last N commits:

```
git log -N
```

Show commit history for last N commits with diff:

```
git log -p -N
```

See who changed and what in a file:

```
git blame <file>
```

See changes to file over time:

```
git log -p <file>
```

Show remote branches and their mapping to local:

```
git remote show origin
```

## Branches

List all local branches:

```
git branch
```

List all remote branches:

```
git branch -a
```

List all existing branches:

```
git branch -av
```

Create local branch and switch to it:

> If you don't want to switch remove -b

```
git checkout -b <branch name>
```

Switch to existing branch:

```
git checkout <branch name>
```

Rename current branch:

```
git branch -m <new name>
```

Delete a local branch:

```
git branch -d <branch name>
```

## Merge

To merge branch to origin:

```
git merge <branch name>
```

## Tags

Get remote tags:

```
git pull --tags
```

Switch to an existing tag:

```
git checkout <tag name>
```

List all tags:

```
git tag
```

Create new tag

```
git tag -a <tag name> -m "COMMENT"
```

Push all tags to remote repository:

```
git push --tags
```

## Clean and undo

Discard all changes in working directory:

```
git reset --hard <some commit>
```

Discard local changes in file:

```
git checkout <some commit> <file>
```

Delete all untracked files:

```
git clean -f
```

Delete all untracked files and directories:

```
git clean -df
```

Undo local modifications to all files:

```
git checkout -- .
```
