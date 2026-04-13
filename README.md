



# Basic git commands

* Git in it: will intiate a new repository in current directy
* git clone: will clone the repo from remote URL to your local machine
* git status: will show the working directory status(which files are modified, added, stagged, etc)
* git add : stages a file or files to be commited
* git commit -m "Message": commit staged changes to the local repo with message

* git push : pushes commited changes to the remote repository

* git pull: fetches and merges changes from the remote repo to your current branch
* git fetch: download changes from remote repo with out merging them in to your current branch
* git merge: combine changes from one branch in to the other branch

* git log: shows the commit history of the repository

* git diff: show the diff b/w your current working directory and the index

# Branching commands(Managing branches)

* git branch: Lists all the branches in the repository
* git branch <branch_name>: create a new branch
* git checkout <branch_name>: switches to an existing branch
* git checkout -b <branch_name>: creates and switches to a new branch in one step
* git merge <branch_name>: merges changes from one branch in the other branch
* git rebase<branch_name>: applies changes from one branch on to the other branch(instead of merging).
* git branch -d <branch_name>: Delete the specified branch locally
* git branch -D <branch_name>: Forcefully deletes a branch locally
* git remote set-head origin<branch_name>: set the default branch for the remote repo

# Remote commands (managing the remotes and syncing the cloud)

* git remote -v: shows remote repo URLS
* git remote add: Adds a new remote repository
* git remote remove: removes a remote repository
* git push origin <branch>: push a branch to a remote repository
* git push -u origin<branch_name>: pushes branch to the remote repository and sets the upstream for the branch.
* git pull origin <branch_name>: fetches and merges the changes from remote repo to current branch
* git fetch origin: downlaod changes from the remote repo
* git remote show origin: shows the detail information about a remote repository

# staging and commiting (managing changes)

* git add . : stages all modifies files in the working directory
* git add -A: stages all modifies files(including the file deletions)
* git reset: unstages a file(reverts it to the working directory)
* git commit --amend: modifies the last commit(can change the commit message or add changes)
* git commit --all: Automatically stages tracked files and commits them.
* git commit -a: stages and commits all modified files
* git commit --no-verify: skips pre-commit hooks while commiting
* git reset --soft HEAD~1?: moves the HEAD pointer back one commit but leaves your changes staged
* git reset --hard HEAD~1: Moves the HEAD pointer back one commit and discards changes in the working directory