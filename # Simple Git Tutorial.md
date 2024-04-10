# Simple Git Tutorial

This tutorial covers the basics of using Git for version control. Git allows you to track changes, revert to previous states, and collaborate with others on projects. This guide assumes you have Git installed and a basic understanding of its purpose.

## Getting Started

- **Watch Inside Hidden .git Folders:** To see the contents of the `.git` directory which contains all the metadata for the repository's history, use the command:
ls -a .git


## Making Changes to the Repository

- **Add Changes:** To add a specific file to the staging area (mark it for inclusion in the next commit):
git add <filename.filetype>


- **Add All Changes:** To add all new or modified files to the staging area:
git add --all


## Saving Changes

- **Commit Changes:** To save your changes to the local repository with a message describing what was changed:
git commit -am "description of changes"


## Checking Status

- **Check Status:** To see which files have been modified and staged for commit:
git status


## Checking Earlier Versions

- **View Commit History:** To see the commit history of a specific file, along with commit messages:
git log <filename.filetype>

It's important to commit often to keep track of changes.

- **Seeing Actual Changes of Files:** To see the detailed changes (patches) made to a file:
git log -p <filename.filetype>

## Going Back to Earlier Versions

- **Checkout a Previous Commit:** To revert files in your working directory to a previous state:
git checkout <commit hash>


- **Commit the Reverted Changes:** It's good practice to commit this action with a message:
git commit -am "restore earlier version"


## Working with Branches

- **Creating a New Branch:** To create a new branch and switch to it:
git checkout -b <new branch name>


- **Checking Current Branch:** The `git status` command will tell you which branch you're on.

- **List All Branches:** To see all branches in your repository:
git branch


- **Deleting a Branch:** To delete a branch:
git branch -D <branch name>

- **Switching Back to the Main Branch:** To switch back to the main branch:
git checkout master


- **Merging Branches:** To merge changes from one branch into another (e.g., merging a feature branch into the main branch):
git merge <branch name>

Be aware that working on several branches simultaneously can cause merge conflicts.

## Pushing Changes to GitHub

- **Initial Push to GitHub:** To push your local repository to GitHub for the first time:
git remote add origin git@github.com:YourUsername/repository_name.git
git push -u origin <branch name>


- **Pushing Changes After the First Time:** To push changes after the initial setup:
git push origin <branch name>


## Pulling from GitHub

- **Cloning a Repository:** To copy a repository from GitHub to your local machine:
git clone https://github.com/YourUsername/repository_name.git






