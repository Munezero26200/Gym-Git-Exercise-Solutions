
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

## Bundle3
### Exercise1
```bash


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)Documents/Git_Exercises_Project (ft/service-redesign)
$ git push origin ft/service-redesign     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.       
Delta compression using up to 2 threads   
Compressing objects: 100% (3/3), done.    
Writing objects: 100% (3/3), 544 bytes | 272.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:      
remote:      https://github.com/Munezero26200/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean     

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git find . services.html
git: 'find' is not a git command. See 'git --help'.

The most similar command is
        init

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ find . services.html
.
./.git
./.git/COMMIT_EDITMSG
./.git/config
./.git/description
./.git/FETCH_HEAD
./.git/HEAD
./.git/hooks
./.git/hooks/applypatch-msg.sample        
./.git/hooks/commit-msg.sample
./.git/hooks/fsmonitor-watchman.sample
./.git/hooks/post-update.sample
./.git/hooks/pre-applypatch.sample        
./.git/hooks/pre-commit.sample
./.git/hooks/pre-merge-commit.sample      
./.git/hooks/pre-push.sample
./.git/hooks/pre-rebase.sample
./.git/hooks/pre-receive.sample
./.git/hooks/prepare-commit-msg.sample
./.git/hooks/push-to-checkout.sample      
./.git/hooks/sendemail-validate.sample    
./.git/hooks/update.sample
./.git/index
./.git/info
./.git/info/exclude
./.git/logs
./.git/logs/HEAD
./.git/logs/refs
./.git/logs/refs/heads
./.git/logs/refs/heads/dev
./.git/logs/refs/heads/ft
./.git/logs/refs/heads/ft/bundle-2        
./.git/logs/refs/heads/ft/service-redesign./.git/logs/refs/heads/main
./.git/logs/refs/heads/switch
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/logs/refs/remotes/origin/dev       
./.git/logs/refs/remotes/origin/ft
./.git/logs/refs/remotes/origin/ft/service-redesign
./.git/logs/refs/remotes/origin/HEAD      
./.git/logs/refs/remotes/origin/main      
./.git/logs/refs/stash
./.git/objects
./.git/objects/01
./.git/objects/01/9f33277f463af458be8a8d1cefc3ed3e6d37fc
./.git/objects/14
./.git/objects/14/7c1c8046975a7d87d00d2d611ca543326001ce
./.git/objects/19
./.git/objects/19/ea8d895eed829291b8c59c420fa1717fb6c827
./.git/objects/1f
./.git/objects/1f/d8dda0a83228edad2ef21f817f84fefb72eba2
./.git/objects/23
./.git/objects/23/6c15f068df43474dd93a26c4b5f46c61fcaf38
./.git/objects/2e
./.git/objects/2e/077b5d3ec346062d06c61a96aa1e07e7767973
./.git/objects/31
./.git/objects/31/5950a2589d6b40d07b5a16ae1f6b120d8ea849
./.git/objects/39
./.git/objects/39/d97b1b81d1c281105b0986a90158c8ee24c336
./.git/objects/40
./.git/objects/40/805b4bae177ba2acc46ccd265ca380ab79db85
./.git/objects/41
./.git/objects/41/b4e2043735a89b5a548764c7ade6282cfa3deb
./.git/objects/43
./.git/objects/43/8ef84234fef6eaf459477675e1015ecb52e3d0
./.git/objects/49
./.git/objects/49/5d7a9625dd33eb8116f1be4d320c3cc885d9c4
./.git/objects/4a
./.git/objects/4a/91ea6409ea73b0be111cd189ce5e9cd99312b6
./.git/objects/4b
./.git/objects/4b/ed05f2018e143e98b97002bd25b5e8f5e08062
./.git/objects/59
./.git/objects/59/fa1bfe14250258c31ef1d07359c6722f02e842
./.git/objects/5b
./.git/objects/5b/a09e5cf717d0caf47b7aa38f9105d421858e85
./.git/objects/5d
./.git/objects/5d/5c6d7a0c6e96e89f3ad956fa9aaaf1ef74d6e3
./.git/objects/5d/8ed4978f621e2ac41b5b7d8aceaf4daf0fd1d3
./.git/objects/61
./.git/objects/61/bff26dc22f9ed598b529cb498afc30406207d7
./.git/objects/62
./.git/objects/62/201769892855d645a9c4429b461aa1d6fa7379
./.git/objects/62/974c847ed933d9e401805eae298636111e9e49
./.git/objects/65
./.git/objects/65/12b8a6730a7512d4546bca7b15c65216cf7877
./.git/objects/69
./.git/objects/69/85b14273afa6a656344f9ea9e35734a51c0033
./.git/objects/6b
./.git/objects/6b/66dc6c88ddc9cbd1c7161e4f3ba727afa6f11b
./.git/objects/7e
./.git/objects/7e/91168f4bf33bf6db7df0e6a77f6fb1daf290b2
./.git/objects/7f
./.git/objects/7f/c083b28ffcac25cea88ddc287dd95be9194903
./.git/objects/8b
./.git/objects/8b/e4168d880b603adfaf48cb91eb26879c0304be
./.git/objects/8d
./.git/objects/8d/d7fb881e7fe1bc3ff04b45c467e4641a2aae91
./.git/objects/8f
./.git/objects/8f/6d4dc17b1927f5f4a0d4f058db77dcb0f1272b
./.git/objects/90
./.git/objects/90/7706083cc6541c5e68d44e8986cb6c57fc3841
./.git/objects/94
./.git/objects/94/678160e1981696db30ba5fd8bbfc351c1d0c71
./.git/objects/97
./.git/objects/97/92778b28176cd18725705de39dcc4c08eb2f41
./.git/objects/98
./.git/objects/98/79f376e51cbb99b5f60db716f80f3e0c58b964
./.git/objects/9b
./.git/objects/9b/9eef696f9cd4eaa191e58fc410b33a258dc1d6
./.git/objects/a1
./.git/objects/a1/a75496a8356d34097b4d76dc6a764e33be01eb
./.git/objects/a5
./.git/objects/a5/bb63db79da8d6083f0b0d73bec4b25497457dc
./.git/objects/a7
./.git/objects/a7/b140206c01eed2cde35e29fb44220f0f183e8f
./.git/objects/ab
./.git/objects/ab/0b277ab20971f6496e74600dfe9bddcac21e6a
./.git/objects/b2
./.git/objects/b2/4602fb014b6f01e9c9c5c70be2c4daed620070
./.git/objects/b5
./.git/objects/b5/197ea3404566e2a09e5451024a6da55baaf379
./.git/objects/b5/6b28e2f691ebeef831dac1bb3f8d7f47107b88
./.git/objects/b8
./.git/objects/b8/c6f59216b948629a7386173b7b7136314f29cc
./.git/objects/ba
./.git/objects/ba/a5a78a2455c52d0e3924c50d7bb85a294367b5
./.git/objects/bb
./.git/objects/bb/349f8a9410a897bf9c40559bba4a189fdcef6c
./.git/objects/c1
./.git/objects/c1/5f1f54b45635b297891bf52d5824ed8589b64a
./.git/objects/c2
./.git/objects/c2/c1732676c70430ed12417dc21da91d9914df52
./.git/objects/c5
./.git/objects/c5/3aad38e1ee340256c7b5950be08a7cac5197a1
./.git/objects/ca
./.git/objects/ca/fa3d5069f803ce10c3a7bb34b9349f32e411d2
./.git/objects/cd
./.git/objects/cd/872ab868608c7150db55cbd64192a61d7db2ac
./.git/objects/cd/effb549b0e3fef6cf9e7ec3550a0cc0d2fa25c
./.git/objects/d0
./.git/objects/d0/4a7887054fc28723faa9499c63bbd1be07fdfd
./.git/objects/d8
./.git/objects/d8/537ae8b120a2585cecbd17a6729c3af2333273
./.git/objects/df
./.git/objects/df/a2c4b4794730cb8c3b4ba61da46a367b50cef1
./.git/objects/e5
./.git/objects/e5/d901daed035d57e0c4dfffdeaddd677789c9cd
./.git/objects/f1
./.git/objects/f1/f208da3e374ef30c1655d0293257fb836debcd
./.git/objects/fc
./.git/objects/fc/bc0569b1bfb1c7d726ee72d4d58ca8c3a975c4
./.git/objects/fc/e0fef5a7a0851b4a5298a166dbb965004b1b17
./.git/objects/fd
./.git/objects/fd/8b7012623d0f8c0c7d9b410d19d7afdb78c294
./.git/objects/fe
./.git/objects/fe/21ad80d42f9c4594230efdb69aabf52a9bfa0a
./.git/objects/ff
./.git/objects/ff/001cb29b26761eafa716e98e0e6b2c49f7e31c
./.git/objects/info
./.git/objects/pack
./.git/ORIG_HEAD
./.git/refs
./.git/refs/heads
./.git/refs/heads/dev
./.git/refs/heads/ft
./.git/refs/heads/ft/bundle-2
./.git/refs/heads/ft/service-redesign     
./.git/refs/heads/main
./.git/refs/heads/switch
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/refs/remotes/origin/dev
./.git/refs/remotes/origin/ft
./.git/refs/remotes/origin/ft/service-redesign
./.git/refs/remotes/origin/HEAD
./.git/refs/remotes/origin/main
./.git/refs/stash
./.git/refs/tags
./index.html
./README.md
./services.html
services.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)Documents/Git_Exercises_Project (ft/service-redesign)
$ git checkout main --./services.html
error: unknown option `./services.html'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --[no-]guess          second guess 'git checkout <no-such-branch>' (default)    
    --[no-]overlay        use overlay mode (default)
    -q, --[no-]quiet      suppress progress reporting
    --[no-]recurse-submodules[=<checkout>]                          control recursive updating of submodules
    --[no-]progress       force progress reporting
    -m, --[no-]merge      perform a 3-way 
merge with the new branch
    --[no-]conflict <style>
                          conflict style (merge, diff3, or zdiff3)
    -d, --[no-]detach     detach HEAD at named commit
    -t, --[no-]track[=(direct|inherit)]   
                          set branch tracking configuration
    -f, --[no-]force      force checkout (throw away local modifications)
    --[no-]orphan <new-branch>
                          new unborn branch
    --[no-]overwrite-ignore
                          update ignored files (default)
    --[no-]ignore-other-worktrees
                          do not check if 
another worktree is using this branch     
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --[no-]patch      select hunks interactively
    --[no-]ignore-skip-worktree-bits      
                          do not limit pathspecs to sparse entries only
    --[no-]pathspec-from-file <file>      
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean     

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git add services.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git commit -m "Here is the changes on se
rvices.html file"
On branch ft/service-redesign
nothing to commit, working tree clean     

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git checkout ft/service-redesign        
Already on 'ft/service-redesign'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git checkout main -- templates/services.html
error: pathspec 'templates/services.html' 
did not match any file(s) known to git    

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
new file mode 100644
index 0000000..4a91ea6
--- /dev/null
+++ b/services.html
@@ -0,0 +1,12 @@
+
+<html lang="en">
diff --git a/services.html b/services.htmlnew file mode 100644
index 0000000..4a91ea6                    device-width, initial-scale=1.0">
--- /dev/null
+++ b/services.html
@@ -0,0 +1,12 @@
+                                          command "git branch branch_name"</p>
+<html lang="en">                         name of the branch</p>
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git merge main
Already up to date.

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git commit -m "Here's is the merge of main and  ft/service-redesign"
On branch ft/service-redesign
nothing to commit, working tree clean     

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'   

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)Documents/Git_Exercises_Project (ft/team-page)
$ mkdir  team.html                        Documents/Git_Exercises_Project (ft/team-page)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ rmdir team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)Documents/Git_Exercises_Project (ft/team-page)
$ touch team.html                         Documents/Git_Exercises_Project (ft/team-page)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> ft/team-page


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git commit -m "Here is the changes in team's content file"
[ft/team-page d8a471a] Here is the changes in team's content file
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* ft/team-page
  main
  switch

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.       
Delta compression using up to 2 threads   
Compressing objects: 100% (3/3), done.    
Writing objects: 100% (3/3), 455 bytes | 91.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Munezero26200/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (main)    
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ giy log
bash: giy: command not found

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git log
commit d8a471a20a151a47e5eb9223914107288922e40c (HEAD -> ft/team-page, origin/ft/team-page)
Author: Munezero26200 <alinemunezero920@gmail.com>
ice-redesign)
Author: Munezero26200 <alinemunezero920@gmail.com>                                  file
Date:   Sat May 17 08:51:00 2025 +0200    
                                          b1b17 (origin/ft/service-redesign, ft/service-redesign)
    Here is the changes in services.html fail.com>ile

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/ileDocuments/Git_Exercises_Project (ft/team-page)                                      Documents/Git_Exercises_Project (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git cherry-pick d8a471a20a151a47e5eb9223914107288922e40c
[ft/contact-page 2a017a4] Here is the changes in team's content file
 Date: Sat May 17 09:31:31 2025 +0200     
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ touch contact.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git commit -m "Here's my contact"
[ft/contact-page 076a49c] Here's my contact
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
200/Gym-Git-Exercise-Solutions/pull/new/ft31.00 KiB/s, done./contact-page                             k-reused 0 (from 0)
remote:                                   .
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git                  act-page' on GitHub by visiting:
 * [new branch]      ft/contact-page -> ft200/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page/contact-page
                                          t-Exercise-Solutions.git
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents//contact-pageDocuments/Git_Exercises_Project (ft/contact-page)                                   Documents/Git_Exercises_Project (ft/contact-page)
$ git branch ft/faq-page

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/contact-page)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/faq-page)
$ touch faq.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/faq-page)
$ git add .

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/faq-page)
$ git commit -m "Here is faq.html content"[ft/faq-page e952321] Here is faq.html content
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.       
Delta compression using up to 2 threads   
Compressing objects: 100% (3/3), done.    
Writing objects: 100% (3/3), 451 bytes | 451.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Munezero26200/Gym-Git-Exercise-Solutions/pull/new/ft/ft/faq-page
remote:
To https://github.com/Munezero26200/Gym-Gi-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faqfaq-page

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/
Revert "Here is the changes in team's content file"
age)
$ git revert d8a471a20a151a47e5eb9223914107288922e40c
[ft/team-page 92889ae] Revert "Here is the changes in team's content file"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ push origin ft/team-page
bash: push: command not found

Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/Documents/Git_Exercises_Project (ft/team-page)
$ git push origin ft/team-page
k-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Munezero26200/Gym-Git-Exercise-Solutions.git                  75.00 KiB/s, done.
   d8a471a..92889ae  ft/team-page -> ft/tek-reused 0 (from 0)am-page                                   leted with 1 local object.
                                          t-Exercise-Solutions.git
Admin@DESKTOP-JJ9VPBQ MINGW64 ~/Documents/am-pageDocuments/Git_Exercises_Project (ft/team-p
```