# Git Best Practices

## Basic commands

- Cloning a remote repository to your local computer
    > $ cd /Your/Directory  
    > $ git clone https://<span></span>your-repository.git

- Displaying the state of the working directory  
(such as: current branch, number of commits ahead, modified files, staged files, ...)
    > $ git status

- Updating your local repository with the remote repository
    > $ git pull

- Adding modified files to the stage area
    > $ git add file-1 file-2 file-3  

    Alternatively, you can add all the files at once
    > $ git add .

- Commiting the staged files to your local branch
    > $ git commit -m 'A meaningful commit message'

- Updating the remote repository with your local repository
    > $ git push

<br/>

## How to use branches

A branch represents an independent line of development.  
You can think of them as a way to request a brand new working directory and project history.  
New commits are recorded in the history of the current branch.  
When the work is done, the branch can be marged with the master branch.

<div style="text-align:center">
    <img src="images/branches.png" width="500" />
</div>

- Listing your current local branches
    > $ git branch --list

- Creating new local branch
    > $ git branch your-new-branch-name

- Creating new remote branch
    > $ git push --set-upstream origin your-new-branch-name

- Switching local branches
    > $ git checkout your-new-branch-name

- Deleting local branch
    > $ git branch --delete your-branch-name

- Deleting remote branch
    > $ git push --delete origin your-branch-name
