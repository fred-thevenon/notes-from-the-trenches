# Git Reminder

## Working .gitconfig

```bash
# show email used within a git repository
git config --show-origin --get user.email
```

```text
# working with several .gitconfig : add this to your .gitconfig
[includeIf "gitdir:C:/src/Github/"]
    path = .gitconfig-github
[includeIf "gitdir:C:/src/Work/"]
    path = .gitconfig-work
```

## Working with branches

```bash
# create a new branch and checkout it
git checkout -b new-branch-name
```

```bash
# list local branches
git branch -a
```

```bash
# list remote branches
git branch -r
```

```bash
# list all branches and their remote status
git for-each-ref --format '%(refname) %(upstream:track)'
```

```bach
# how to get a remote branch without checkinout it
git fetch origin test-fetch:test-fetch
```

```bash
# delete a local branch
git branch -d branch-name-to-be-deleted
```

```bash
# delete a remote branch
git push origin --delete branch-name-to-be-deleted
```

```bash
# delete a remote branch
git push origin --delete branch-name-to-be-deleted
```

## Working with merge

```bash
# list merged branches in main branch
git --merged main
```

```bash
# list non merged branches in main branch
git --no-merged main
```

```bash
# merge witout merged commit
git merge --ff-only super-feature-branch-name
```

```bash
# how to rebase your feature branch
# pull the main branch
# checkout your feature branch
git rebase main
```

## Housekeeping

```bash
# update your local list of remote branches
git fetch --prune
```

## Worktree

```bash
git worktree add -b chore/514-init ../projectwt/514-init
```
