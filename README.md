## This is a repository for learning Git

## Commands used

- git init: create a new repository.
- git status: Compare working directory, stating area and current branch.
- git add: Add changes from working directory to staging area.
- git commit: Commit changes from staging area to current branch.
- git config: Set or get configuration.

- git branch -c <branch name>: Create a Branch.
- git checkout <branch name>: Checkout (change to) to a particular branch. update HEAD and apply changes to working directory.
- git checkout -b <branch name>: Create branch, then check it out
- git branch -v: shows the branches with most recent commit information.
- git branch --no-merged branch1: List branches that have unmerged commits with the given branch.
- git branch --merged branch1: List branches that have no unmerged commits with the given branch.

- git stash: Stash changes from  working directory
- git stash list: list stashes across all the branches
- git stash pop: Apply stashed changes to working directory

- git log: Show history of project commits on the current branch.
- git log: Shows the log in the current branch.(newly added)
- git log --all: This shows commits on all the branches
- git log <branch name>: Shows commits on the specified branches
- git log <commit id>: Shows commits prior to the given commit id
- git log --author "Bhimavarapu": shows commits by a specific author.
- git log --since "last 2 hours": shows commits since last 2 hours.
- git log --until "July 5": shows commits until the specified day.
- git log --oneline: commits displayed in a single line (compact view).
- git log --oneline --graph --all: shows commits in graphical representation for all the branches.
- git log branch1..branch2: Log of commits in branch2 that don't exist in branch1.
- git log branch1...branch2: Log of commits in either branch but not both.

- git show <commit id>: shows the changes made via the specific commit ID in detail.

- git merge: Merge commits from two different branches.
- git merge --abort: Abort an in-progress merge.
- git merge --no-commit --no-ff: Attempt to merge, but don't create an auto merge or ff merge.

- git remote -v: List remote repositories
- git remote add `remote` `git path`: Add a new `remote` at `url`.
- git push -u `remote` `branch`: Push `branch` to `remote`, and set default upstream for the `branch`.
- git fetch: Fetch the updates from `remote`
- git pull: Fetch and then merge

just did a ff merge with remote-commands branch

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch. When we make a commit while we're on a Branch, the branch is updated to ref(er) to the new commit.

## What's HEAD?

HEAD is a ref(rence) to the "current" branch(or sometimes a commit...more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates the HEAD to ref(er) to a different branch.

## Commit messages

Default editor is vim(this can be changed)
 - `i` to enter *insert* mode
 - Type commit message
 - `Esc` -> `:wq` -> `Enter` to write message and quit Or use 'git commit -m <"message">'
 - First line should be clear, accurate, and concise
 - Use proper spelling, grammar and punctuations.
 Don't end with a `.`.

 For more advice, see: https://chris.beams.io/posts/git-commit/

## Merging

Merging means to bring the changes from one branch into another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.

## What's a remote?

A remote repo is one hosted somewhere other than on our local machine. We can add remotes with `git remote add`, and set up *tracking branches* to track differences between out local and remote repositories.

We push to remotes with `git push`, and fetch from them with `git fetch`. We can also fetch and merge in one set with `git pull`.
