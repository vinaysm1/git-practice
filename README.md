##This is a repository for learning Git

##Commands used

- git init: create a repository.
- git status: Compare working directory, stating area and current branch.
- git add: Add changes from working directory to staging area.
- git commit: Commit changes from staging area to current branch.
- git config: Set or get configuration.
- git log: Show history of project commits
- git branch -c: Create a Branch.
- git checkout: Checkout (change to) to a particular branch.
- git checkout -b: Create branch, then check it out
- git stash: Stash changes from  working directory
- git stash list: list stashes
- git stash pop: Apply stashed changes to working directory

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch. When we make a commit while we're on a Branch, the branch is updated to ref(er) to the new commit.

## What's HEAD?

HEAD is a ref(rence) to the "current" branch(or sometimes a commit...more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates the HEAD to ref(er) to a different branch.

## Commit messages

Default editor is vim(this can be changed)
 - `i` to enter *inster* mode
 - Type commit message
 - `Esc` -> `:wq` -> `Enter` to write message and quit Or use 'git commit -m <"message">'

 - First line should be clear, accurate, and concise
 - Use proper spelling, grammar and punctuations.
 Don't end with a `.`.

 For more advice, see: https://chris.beams.io/posts/git-commit/
