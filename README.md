# Git Practice Repository

## Commands

- git init: Create a repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: set or get configuration stored in system, local, global, worktree, or file
- git log: show history of project commits in descending order
- git branch: List branches
- git checkout: check out a branch (update HEAD)
- git checkout -b: Create branch, and then check it out

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch. When we make a commit while we're on a branch, the branch is updated to ref(er) to the new commit.

## What's HEAD?

HEAD is a ref(erence) to the "current" (or sometimes a commit...more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates HEAD to ref(er) to a different branch.

## Commit Messages

Default editor is vim but can be changed
 - `i` to enter *insert* mode
 - Type commit message
 - `Esc` -> `:wq` -> `Enter` to write message and quit
Or use `git commit -m "<message text/line"`
