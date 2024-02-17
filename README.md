# Git-Course

Git Commands
------------

git --version

Git : Configurations:
-------------------
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

Git : Starting a repository
---------------------------
git init -> initialise the folder/project to use git
git status -> check status of the changes

Git : staging files
-------------------
git add . -> adds all the progress/changes to be saved to the staging area.
git add <filename> -> adds the mentioned files to be saved to the staging area.
git add <filename> <filename1> <filename2> ..
git add -all
git add -A
git rm --cached <filename>
git reset <filename>

Git : Commiting to repository
-----------------------------
git commit -m "message"->  save changes with message
git reset --soft HEAD^
git commit --amend -m <message>
git commit -a -m <message> -> commit the changes without tracking/staging.

Git : Commiting to repository
-----------------------------
git remote add origin <git url> -> attach remote repository to current git project/folder

git push -> move the saved changes from sytem to the current checedout remote repository
git push origin <branch name>-> move the changes in the branch from sytem to remote, creates the new branch in the remote repository
git push origin <branch name>-> move the changes in the branch from sytem to remote, creates the new branch in the remote repository
git pull origin <branch name> -> pulls the changes from remote branch to the local branch 


git log -> see all previous changes, it's a log of all the changes captured.
git checkout <commit_id> -> checkout a particular commit, this will move us back to earlier state of the commit id

git checkout -b <branch-name> -> creates a new branch with branch name provided
git branch -> list the branches
git push origin <branch name>-> move the changes in the new branch from sytem to remote, creates the new branch in the remote repository

git diff -> check the changes made to files in the working directories
git diff --staged -> check teh changes made to files once added to staging area.


git clone -b <branchname> <git url>

git push -u origin main

<>
$ git remote add origin <git url>

<>
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

==============================================
Adding SSH Keys
==============================================
Command Syntax : ssh-keygen -o
cd ~/.ssh
cat id_rsa.pub
copy content and paste in gitgub -> settings -> ssh -> newSSHkeys -> paste
