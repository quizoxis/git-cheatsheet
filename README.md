# Git Practice Repository

## Commands

- git init: Create a repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: set or get configuration stored in system, local, global, worktree, or file
- git log: show history of project commits in descending order
- git checkout: Check out branch (update HEAD and apply changes) to working directory
- git merge: Merge changes from different branches

## Commit Messages

Default editor is vim but can be changed
 - `i` to enter *insert* mode
 - Type commit message
 - `Esc` -> `:wq` -> `Enter` to write message and quit
Or use `git commit -m "<message text/line"`

## Merging

Merging means to bring the changes from one branch into another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
