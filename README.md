
# Git Exercises
## Bundle 1
### Exercise1
```bash
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project
$ git init
Initialized empty Git repository in C:/Users/Admin/Documents/Documents/Git_Exercises_Project/.git/

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (master)
$ touch README.md

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (master)
$ git branch -M master main

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git remote add origin https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git push -u main
error: src refspec refs/heads/main does not match any
error: failed to push some refs to 'main'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git commit -m "Initial commit"
[main (root-commit) 019f332] Initial commit
 1 file changed, 5 insertions(+)
 create mode 100644 README.md

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git push -u main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$  git push --set-upstream origin main
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git pull origin main --rebase
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 367 bytes | 6.00 KiB/s, done.
From https://github.com/Munezero26200/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git push -u main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$   git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
   62974c8..5d5c6d7  main -> main
branch 'main' set up to track 'origin/main'.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git checkout -b test
Switched to a new branch 'test'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (test)
$ git switch dev
Switched to branch 'dev'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git branch -D test
Deleted branch test (was 5d5c6d7).

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git branch
* dev
  main

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$
```
### Exercise2
```bash
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
   c53aad3..fe21ad8  main -> main

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git branch switch dev

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git  switch dev
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git switch dev
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git branch
  dev
* main
  switch

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git switch dev
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git checkout dev
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git stash
Saved working directory and index state WIP on main: fe21ad8 second commit

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git branch switch dev
fatal: a branch named 'switch' already exists

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git branch 
  dev
* main
  switch

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)
$ git switch dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git commit -m 'second commit'
[dev 438ef84] second commit
 1 file changed, 1 insertion(+), 1 deletion(-)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git commit -m 'last changes'
[dev baa5a78] last changes
 1 file changed, 1 insertion(+), 1 deletion(-)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 638 bytes | 212.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
   5d5c6d7..baa5a78  dev -> dev

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$
 *  History restored 

$ git stash
No local changes to save                                    cises_Project (dev)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
cises_Project (dev)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)cises_Project (dev)
$ git stash                                                 last changes
Saved working directory and index state WIP on dev: baa5a78 
last changes                                                cises_Project (dev)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash
Saved working directory and index state WIP on dev: baa5a78 
last changes

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash
Saved working directory and index state WIP on dev: baa5a78 
last changes

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (6512b8a6730a7512d4546bca7b15c65216cf7877)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash list
stash@{0}: WIP on dev: baa5a78 last changes
stash@{1}: WIP on dev: baa5a78 last changes
stash@{2}: WIP on main: fe21ad8 second commit

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html
        new file:   team.html

Dropped stash@{1} (59fa1bfe14250258c31ef1d07359c6722f02e842)
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git commit -m "init project"
[dev 40805b4] init project        
 2 files changed, 23 insertions(+)
 create mode 100644 home.html
 create mode 100644 team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
 that you do not
hint: have locally. This is usually caused by another reposins.gittory pushing to
hint: the same ref. If you want to integrate the remote chanero26200/Gym-Git-Exercise-Solutions.git'ges, use                                                     that you do not
hint: 'git pull' before pushing again.                      tory pushing to
hint: See the 'Note about fast-forwards' in 'git push --helpges, use' for details.
                                                            ' for details.
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)                                         cises_Project (dev)
$ git pull origin dev --rebase
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.01 KiB | 9.00 KiB/s, done.
From https://github.com/Munezero26200/Gym-Git-Exercise-Solutions
 * branch            dev        -> FETCH_HEAD
   baa5a78..495d7a9  dev        -> origin/dev
Successfully rebased and updated refs/heads/dev.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 591 bytes | 591.00 KiB/s, done.Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
   495d7a9..b5197ea  dev -> dev

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git push
Everything up-to-date

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash list
stash@{0}: WIP on dev: baa5a78 last changes
stash@{1}: WIP on main: fe21ad8 second commit

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{0} (e5d901daed035d57e0c4dfffdeaddd677789c9cd)
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   index.html

The stash entry is kept in case you need it again.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop stash@{1}
fatal: log for 'stash' only has 1 entries

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git stash pop stash@{0}
index.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git statuss
git: 'statuss' is not a git command. See 'git --help'.

The most similar command is
        status

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   index.html


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)cises_Project (dev)
$ git add index.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git commit -m "Resolved conflict"
[dev d8537ae] Resolved conflict
 1 file changed, 11 insertions(+)
 create mode 100644 about.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 434 bytes | 434.00 KiB/s, done.Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
   b5197ea..d8537ae  dev -> dev

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$ git reset team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (dev)
$
```
