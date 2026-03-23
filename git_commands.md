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


