This is the content

**git add** file name for particular file
**git add .** for adding all the file which created or modified in the current repo main.
**git commit** -m "Message for the commit which you have done"

These three are the basic comment for after git configure 

addidng one extra line to check the git diff command 

**git push to push the code to remote repositories
git pull to pull the latest to local repository**

adding some new content to check the git diff command 
**git diff command is used to check the changes before add and commit
git diff --cached comand used to check the added changed in staging before commit**


Renamed the file name from Example2.tx to NewName.txt to check the git status


Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    Example2.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        NewName.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Anbu1\git_Essential_training>   After Git add name is showing as renamed  
PS C:\Users\Anbu1\git_Essential_training> git add .
PS C:\Users\Anbu1\git_Essential_training> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    Example2.txt -> NewName.txt

PS C:\Users\Anbu1\git_Essential_training>  Changing the filename from cli

PS C:\Users\Anbu1\git_Essential_training>** git mv .\Example.md Rename.md**
PS C:\Users\Anbu1\git_Essential_training> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    Example.md -> Rename.md

Creating the new folders and checking the status 

I have created the two folder First_Dir and Second_Dir
PS C:\Users\Anbu1\git_Essential_training> git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        First_Dir/

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Anbu1\git_Essential_training> git add .
PS C:\Users\Anbu1\git_Essential_training> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   First_Dir/Second_samplefile.txt
        new file:   First_Dir/first_sample.txt

PS C:\Users\Anbu1\git_Essential_training> 
I have created two directories but the Second_Dir dont have any files. Important git wont track the empty file.
So we have to keep the gitkeepfile inside the folder to make the folder available 

PS C:\Users\Anbu1\git_Essential_training> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   First_Dir/Second_samplefile.txt
        new file:   First_Dir/first_sample.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Second_Dir/

PS C:\Users\Anbu1\git_Essential_training> 
"git restore --staged <file>..." to unstage

git restore . command used to remove the  changes recently made in the repo before add or commit

git log 
git show with commit id

PS C:\Users\Anbu1\git_Essential_training> git log
commit d5030ed56fa4f4fea670c1878a96af7af150b7fe (HEAD -> main, origin/main, origin/HEAD)
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 15:53:03 2026 +0530

    to know about the git restore command

commit 9858af7d242ed9d3f9bf83a75a558762d6e43434
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 15:45:57 2026 +0530

    importance about the gitkeep in empty folder

commit 4e4bc24a2c91045c8db905d65ac175466a8920df
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 15:37:03 2026 +0530

    renamed the file to check and know about the git commands

commit 7270ab44fa455c4665e6396885f67606f0df5e18
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 15:26:42 2026 +0530

    Renamed the file name using the mv command git mv filename

commit a52b670b06bceeb64b55275bbcfb5b341d7b7a57
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 15:24:00 2026 +0530

    Changing the file name into new file name checking the git status from GUI

commit bf4372e35a576b5fe9f3cffa0a10e6fa6a4e2b8e
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 14:49:56 2026 +0530

    git diff

commit fe3ad2788a19d702b4d9c0a61fac8b1cdbc59b2e
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 14:28:30 2026 +0530

    git push and git pull command

commit 06eb0fddab83eed3d60bc28437ed38e9b5e6803e
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 14:16:39 2026 +0530

    git command

commit 09167709c1bab72dca743b9f8f0cfe5f1a91672f
Author: veeranbu <anbuveerapandiyan@gmail.com>
Date:   Mon Mar 23 14:05:59 2026 +0530

    i am commiting the created git files to the local repo using git commit

commit f524cb919d641ae3d2ed029741b68a6dc59ad78f
Author: veeranbu <122789552+veeranbu@users.noreply.github.com>
Date:   Mon Mar 23 12:18:32 2026 +0530

    Initial commit
PS C:\Users\Anbu1\git_Essential_training> git show f524cb919d641ae3d2ed029741b68a6dc59ad78f             
commit f524cb919d641ae3d2ed029741b68a6dc59ad78f
Author: veeranbu <122789552+veeranbu@users.noreply.github.com>
Date:   Mon Mar 23 12:18:32 2026 +0530

    Initial commit

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..8dc38d0
--- /dev/null
+++ b/README.md
@@ -0,0 +1,2 @@
+# git_Essential_training
+git_Essential_trainining
PS C:\Users\Anbu1\git_Essential_training> 
PS C:\Users\Anbu1\git_Essential_training> git log --oneline
3ea278b (HEAD -> main, origin/main, origin/HEAD) git command git log and git show commit id
d5030ed to know about the git restore command
9858af7 importance about the gitkeep in empty folder
4e4bc24 renamed the file to check and know about the git commands
7270ab4 Renamed the file name using the mv command git mv filename
a52b670 Changing the file name into new file name checking the git status from GUI
bf4372e git diff
fe3ad27 git push and git pull command
06eb0fd git command
0916770 i am commiting the created git files to the local repo using git commit
f524cb9 Initial commit
PS C:\Users\Anbu1\git_Essential_training> 

git checkout comit id 
eg :git checkout fe3ad27
it will change the commit to particular commit id for changes 
git checkout main to return to the orginal commit



