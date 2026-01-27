### Bunde1
```

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git branch

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git branch -m master

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (master)
$ git branch -m main

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git add .

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git commit -m"initial commit"
[main (root-commit) fce6b5a] initial commit
 2 files changed, 15 insertions(+)
 create mode 100644 ReadMe.md
 create mode 100644 myHTMLFile.html

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 448 bytes | 7.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git branch dev

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (main)
$ git checkout dev
Switched to branch 'dev'


Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was fce6b5a).

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash push -a
Saved working directory and index state WIP on dev: fce6b5a initial commit

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash push -u -m"about file"
Saved working directory and index state On dev: about file

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash -u -m"this is team page"
Saved working directory and index state On dev: this is team page

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: On dev: this is team page
stash@{1}: On dev: about file
stash@{2}: WIP on dev: fce6b5a initial commit

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{2}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        mySecondHtmlFile.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{2} (8b06a24aeba50c049d917645b816f873ce7a7e27)

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git add .

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git commit -m"here is the mySecondHtmlFile"
[dev a1c50fd] here is the mySecondHtmlFile
 1 file changed, 13 insertions(+)
 create mode 100644 mySecondHtmlFile.html

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 502 bytes | 251.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Munezero26200/Gym-Git-Exercise-Solutions/pull/new/de 
remote:
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: On dev: this is team page
stash@{1}: On dev: about file

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{0}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{0} (d00c05ce0c349c6040cde130fed5a43076f4226a)

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
$ git restore team.html
error: pathspec 'team.html' did not match any file(s) known to git

Admin@MunezeroPC MINGW64 /d/TGX-TS/Gym-Git-Exercise-Solutions (dev)
```