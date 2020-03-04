# Git Commands/Cheatsheet

## Commands

- git init: Create a new repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: set or get configuration stored in system, local, global, worktree, or file
- git log: show history (aka "log") of project commits in descending order
- git show: Show a single commit
- git diff: Show the difference between commits, the working directory, and the staging area
- git checkout: Check out branch (update HEAD and apply changes) to working directory
- git branch -c: Create a branch
- git checkout -b: Create branch, and then check it out
- git branch: List branches
- git merge: Merge changes from different branches
- git remote add <remote> <url>: Add a new <remote> at <url>
- git remote -v: List remote repositories
- git push -u <remote> <branch>: Push <branch> to <remote>, and set default upstream for <branch>
- git fetch: Fetch changes from remote repo

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch. When we make a commit while we're on a branch, the branch is updated to ref(er) to the new commit.

## What's HEAD?

HEAD is a ref(erence) to the "current" (or sometimes a commit...more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates HEAD to ref(er) to a different branch.

- git log: show history of project commits in descending order
- git stash: Stash changes from working directory
- git stash list: List stashes
- git stash pop: Apply stashed changes to working directory

## Commit Messages

Default editor is vim but can be changed
 - `i` to enter *insert* mode
 - Type commit message
 - `Esc` -> `:wq` -> `Enter` to write message and quit
Or use `git commit -m "<message text/line"`

## Merging

Merging means to bring the changes from one branch into another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.
