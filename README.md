# Git Best Practices

## Basic commands

- Cloning a remote repository to your local computer
    > $ cd /Your/Directory  
    > $ git clone https://your-repository.git

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
