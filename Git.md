# Git

Helpful tips for using git.

## Create a new Git repository

```bash
$ git init
$ git add .
$ git commit -m 'Initial commit'
```

## Add a .gitignore

https://github.com/github/gitignore


## Clone an existing project

```bash
# using ssh protocol
$ git clone git@github.com:ssherwood/git-cheatsheet
```

## Stashing changes

```bash
# push uncommitted changes to "stash" stack
$ git stash

# restore the top of the "stash" stack 
$ git stash pop
```

## Reset 

```bash
# abort current uncomitted changes
$ git reset --hard

# restore a specific file to its original state
$ git checkout -- README.md
```

## Staging

```bash
# add everything to staging
$ git add .

# add any files matching a wildcard
$ git add *.java
```

## Committing

```bash
# commit currently staged files
$ git commit -m "<commit message>"

# fix the last commit message
$ git commit --amend
```

* Tips for good commit messages: https://chris.beams.io/posts/git-commit/

## Branching

```bash
# create a new branch
$ git branch [new branch name] [from branch]

# switch branches
$ git checkout <branch name>

# create and switch combined
$ git checkout -b [new branch name] [from branch]
```

## Merging

```bash
# merge from branch into the current branch
$ git merge <from branch>

# explicit merge to/from branches
$ git merge <to branch> <from branch>
```

## Rebasing


## Workflow(s)

* http://reinh.com/blog/2009/03/02/a-git-workflow-for-agile-teams.html


## Useful Tools

* Git Author (for pair/mob commits) - https://github.com/pivotal/git-author
* Git Duet (for pairing) - https://github.com/git-duet/git-duet
