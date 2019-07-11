## This section will talk about basic git remote commands

- git remote -v: shows the available remotes for the current branch.
- git remote add <origin> <https path>: This command will create a new public repository called origin for the current branch you are in.
- git push `origin` master: This command will push the contents of your current branch to the remote master.
- git push -u `origin` master: This command will make the remote repository the default upstream for all future pushes.

- git remove `origin`: This command will remove connection between the remote <origin> and local repository.


## New Project

- There should be a destination `project` available on the git hub/lab before you can push your local repository.
- On the git hub/lab create a `project` to which you want to push your local git repository.
- In the `settings` section of your git hub/lab, `SSH Keys` tab, add the keys of the system from which you will push your local git repository. This is required for successful push.

## Pulling a git hub/lab Project

- on your git bash command prompt run the following.
  `git clone <https path to the hub/lab project>`
