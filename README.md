
# GitHub Commands Test

A sandbox repository for experimenting with Git + GitHub command‑line workflows. Practice branching, merging, rebasing, commits, and remote sync.

## Goals
- Learn branch workflows
- Experiment with commits/merges/rebases
- Test `.gitignore` patterns
- Understand how local and remote stay in sync

## Setup
```bash
git clone https://github.com/xNomadx1/Github-commands-test.git
cd Github-commands-test
```

## Quick Cheat Sheet
```bash
# create a branch
git checkout -b feat/example

# stage & commit
git add .
git commit -m "message"

# push first time / next times
git push -u origin HEAD     # first push from a new branch
git push                    # subsequent pushes

# get updates
git pull --rebase

# merge your branch into main (locally)
git checkout main
git pull --rebase
git merge feat/example
git push

# undo last commit (keep changes staged)
git reset --soft HEAD~1
```

## Notes
Feel free to break things—this repo is for learning.

# GitHub Commands Test

A clean sandbox for learning and experimenting with **Git & GitHub command-line workflows**.  
Use this repo to safely explore branching, merging, rebasing, commits, and remote sync without breaking real projects.

---

## Overview
This repository is your **hands-on Git playground** — designed to help you master version control through real commands and experimentation.  
It’s ideal for developers learning to:
- Create, switch, and merge branches
- Handle commits and pushes
- Resolve conflicts
- Practice proper Git hygiene

---

## Setup
```bash
# Clone this repository
git clone https://github.com/xNomadx1/Github-commands-test.git
cd Github-commands-test
```

---

## Core Concepts
| Concept | Command Example | Purpose |
|----------|-----------------|----------|
| Check branch/status | `git status` | See what’s changed locally |
| Create new branch | `git checkout -b feat/test` | Start new work safely |
| Stage & commit | `git add . && git commit -m "message"` | Record changes |
| Push branch to remote | `git push -u origin feat/test` | Upload branch |
| Merge into main | `git checkout main && git merge feat/test` | Combine work |
| Update from remote | `git pull --rebase origin main` | Sync with latest |
| Delete branch | `git branch -d feat/test` | Clean up locally |

---

## Useful Git Tips
- View commit history visually:
  ```bash
  git log --oneline --graph --decorate
  ```
- Undo your last commit (keep changes staged):
  ```bash
  git reset --soft HEAD~1
  ```
- See what changed before committing:
  ```bash
  git diff
  ```
- Recover lost commits:
  ```bash
  git reflog
  ```

---

## Pro Tips
- Keep commit messages clear and descriptive.  
- Avoid force-pushing to shared branches unless absolutely necessary.  
- Always pull with `--rebase` to maintain a cleaner history.  
- Break things here, **not** in production — this repo is your lab.

GitHub Commands Test
--------------------
A sandbox repository for experimenting with Git and GitHub command-line workflows.  
Use this project to explore branching, merging, rebasing, commits, and remote sync in a clean and controlled environment.

Overview
--------
This repository is intended for hands-on Git practice.  
It helps you learn how to:
- Create, switch, and merge branches
- Stage and commit changes
- Push and pull from remote repositories
- Resolve conflicts
- Maintain clean commit history

Setup
-----
Clone this repository to your local machine:
```
git clone https://github.com/xNomadx1/Github-commands-test.git
cd Github-commands-test
```

Core Concepts
-------------
Concept | Command Example | Purpose
--------|-----------------|---------
Check branch/status | git status | View local changes and branch info
Create new branch | git checkout -b feat/test | Start new work safely
Stage and commit | git add . && git commit -m "message" | Record changes
Push branch to remote | git push -u origin feat/test | Upload branch
Merge into main | git checkout main && git merge feat/test | Combine work
Update from remote | git pull --rebase origin main | Sync with latest version
Delete branch | git branch -d feat/test | Clean up local branches

Useful Git Tips
---------------
View commit history visually:
```
git log --oneline --graph --decorate
```

Undo your last commit but keep changes staged:
```
git reset --soft HEAD~1
```

See what changed before committing:
```
git diff
```

Recover lost commits:
```
git reflog
```

Pro Tips
---------
- Keep commit messages short and meaningful.
- Avoid force-pushing to shared branches unless absolutely necessary.
- Use rebase instead of merge for cleaner history.
- This repository is for learning—experiment freely.

Learning Git through experimentation, iteration, and clean commits.