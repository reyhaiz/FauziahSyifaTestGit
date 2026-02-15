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


Proof of work
C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git init
Initialized empty Git repository in C:/Users/ASUS/IdeaProjects/FauziahSyifaTestGit/.git/

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        .idea/
        build.gradle
        gradle/
        gradlew
        gradlew.bat
        settings.gradle

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>notepad README.md

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git add .
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'build.gradle', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'gradlew', LF will be replaced by CRLF the next time Git touches it

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git commit -m "Initial commit with README"
[master (root-commit) 4b8f933] Initial commit with README
 11 files changed, 496 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 .idea/.gitignore
 create mode 100644 .idea/gradle.xml
 create mode 100644 .idea/misc.xml
 create mode 100644 README.md
 create mode 100644 build.gradle
 create mode 100644 gradle/wrapper/gradle-wrapper.jar
 create mode 100644 gradle/wrapper/gradle-wrapper.properties
 create mode 100644 gradlew
 create mode 100644 gradlew.bat
 create mode 100644 settings.gradle

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git log --oneline
4b8f933 (HEAD -> master) Initial commit with README

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git remote add origin https://github.com/reyhaiz/FauziahSyifaTestGit.git

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git remote -v
origin  https://github.com/reyhaiz/FauziahSyifaTestGit.git (fetch)
origin  https://github.com/reyhaiz/FauziahSyifaTestGit.git (push)

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git push -u origin master
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (16/16), 60.62 KiB | 4.66 MiB/s, done.
Total 16 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/reyhaiz/FauziahSyifaTestGit.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .idea/gradle.xml
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .idea/vcs.xml

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git add README.md

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git commit -m "Fix README"
[master ec47588] Fix README
 1 file changed, 1 insertion(+), 32 deletions(-)

C:\Users\ASUS\IdeaProjects\FauziahSyifaTestGit>git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 482 bytes | 482.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/reyhaiz/FauziahSyifaTestGit.git
   4b8f933..ec47588  master -> master

