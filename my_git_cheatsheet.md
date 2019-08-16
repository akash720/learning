* git help **command** -> for help on **command**

* git init -> initialize empty repo

* git remote add **remotename** **remoteURL**-> to add remote with name **remotename** as a reference to **remoteURL**

* git add **filename** -> to track(*OR* add) the **filename** present in CWD

* git add -A -> to track(*OR* add) all the files in entire directory

* git reset HEAD **filename** *OR* git reset -> to unstage changes which are ready to be committed

* git clean -f	-> to remove untracked files

* git commit -m **message** -> to commit files with **message**

* git log -> show commits log

* git status -> show status of working tree like unstaged files, tracked files, etc

* git whatchanged -> show logs with changes

* git checkout -- **filename** -> to discard changes of unstaged **filename** in CWD

* git branch **branch_name** -> create new branch with name **branch_name** without checkout

* git branch -a -> show all branches(local + remote-tracking) (https://stackoverflow.com/questions/10588291/git-branching-master-vs-origin-master-vs-remotes-origin-master)

* git checkout -b **branch_name** -> create and change branch to **branch_name**

* git checkout **branch_name** -> change branch to **branch_name**

* git branch -d **branch_name** -> to delete ONLY local branch having name **branch_name** 

* git push origin --delete **branch_name** -> to delete **ONLY** remote branch with name **branch_name**

* git pull **remote branch** = git fetch + git rebase **remote/branch**

* git fetch **remote** -> download the files from all branches of **remote**

* git fetch **remote branch** -> only download the files of **branch** specified

* git merge **branch** -> incorporates changes from the **branch** into the current branch checked out

* git rebase **branch** -> reapply commits of current branch on top of the base of **branch** specified

* git diff **branch1..branch2** -> show differences between both branches

* git diff **commit1 commit2** -> show differences between both commits

* git config help.autocorrect 1 -> will autocorrect a typo in command

* git reset --soft HEAD^ -> will keep your changes and revert to last(most recent) commit

* git reset --hard HEAD^ -> will not keep your changes and revert to last(most recent) commit

* git reset --hard **commit_id** -> will not keep your changes and revert to the commit referred by **commit_id**

* git stash -> saves your uncommited local changes

* git stash apply -> apply your local changes but the stash will not be deleted

* git stash pop -> apply your local changes but the stash will be deleted

* git revert HEAD -> used for reverting or undo the latest commit

* git revert **commit_id(s)** -> used for reverting the **commit_id(s)** specified, i.e. it will revert the changes that the related commit introduced.

* git branch -t **branch1 branch2** -> **branch1** will track **branch2**

------------------------------------------

### NOTES

* Untracked changes are not in Git. Unstaged changes are in Git but not marked for commit. Staged changes are in Git and marked for commit.

* HEAD is a reference to the last commit in the currently check-out branch.
