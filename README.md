
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

