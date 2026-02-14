Git \& GitHub Assignment



Nama: Fauziah Syifa  

Repository: FauziahSyifaTestGit  



Advanced Git Exercise – Part I

1\. What is the difference between git reset and git revert?

`git reset` is used to undo commits by moving the HEAD pointer to a previous commit. This can rewrite history and is best used in local branches.

`git revert` undoes a commit by creating a new commit that reverses the changes from a previous commit. This is safer when working in a team.



2\. What is the difference between git merge and git rebase?

`git merge` combines branches by creating a merge commit and keeps the full commit history.

`git rebase` rewrites commit history to make it linear and clean. It should not be used on branches that others are working on.



3\. What is the difference between git stash pop and git stash apply?

`git stash apply` applies the stashed changes without removing them from the stash list.

`git stash pop` applies the stashed changes and removes them from the stash list.



4\. What can you do in interactive rebase?

Using interactive rebase, you can:

\- Edit commit messages

\- Reorder commits

\- Squash multiple commits into one

\- Remove commits

\- Modify commit content



Advanced Git Exercise – Part II (Practice)

\- Created local repository using Git

\- Added and committed files

\- Pushed repository to GitHub

\- Forked and cloned the repository from rithmschool

\- Created a feature branch and merged it into main

\- Practiced revert and interactive rebase

\- Submitted pull requests with clean commit history



