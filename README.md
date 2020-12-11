# Git Best Practices

## Basic commands

- Cloning a remote repository to your local computer
    > $ cd /Your/Directory  
    > $ git clone https<nolink>://your-repository.git

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
When the work is done, the new commits can be integrated into the original branch.

<img src="images/branches.png" width="500" />

- Listing your current local branches
    > $ git branch

- Creating new local branch
    > $ git branch your-new-branch-name the-source-branch-name

- Creating new remote branch
    > $ git push -u origin your-new-branch-name the-source-branch-name

- Switching local branches
    > $ git checkout your-new-branch-name

- Deleting local branch
    > $ git branch --delete your-branch-name

- Deleting remote branch
    > $ git push --delete origin your-branch-name

<br/>

## Pull requests

Pull requests are a way to initiate discussions around a branch.  
They give other developers the opportunity to contribute to the new feature before it gets integrated into the official project.

<img src="images/pull-request.png" width="450" />

<br/>

1) In your repository GUI, go to "Pull requests"
2) Select "New pull request"
3) Select the base and target branches
4) Click "Create pull request"
5) Configure the pull request:
    - reviewers: ask people to review your code
    - assignees: assign people to accept your request and merge the branches
    - labels
    - projects
    - milestone
5) Create pull request
6) Once there's nothing more to be done, the feature can be merged by the assigners.

<br/>

## References

- [Basic Git commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)
- [Git branch](https://www.atlassian.com/git/tutorials/using-branches)
- [Pull requests](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)
