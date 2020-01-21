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
