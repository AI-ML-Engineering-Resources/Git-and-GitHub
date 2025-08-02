# Git-and-GitHub
This repository contains the information of Git and GitHub usage. This readme contains the most common Git and GitHub commands used for project management.

## Git
Git is a version control system that keeps track of the changes you made in a specific folder's files (like a history). This specific folder is called a repository. Git works on the your local computer/laptop. Git creates a .git folder that keeps track of all the previous changes. So by using git for your project folder, you can see all the previous changes made, go back to any previous version and much more.

## GitHub
GitHub is an online service where you can store your project folder with the history and share it with anyone. GitHub lets other users access and contribute to your project.

### Git Installation
Download and install Git from [Git site](https://git-scm.com/downloads). Check git install by entering `git --version` on any terminal of your computer. You should get something like `git version 2.45.1.windows.1`. If the terminal cannot recognize the command `git` even after installation, you might need to add the paths of *Git/bin* and *Git/cmd* folders in the environment Variables for Windows Users.

### Git Configuration
Add your name and email to the git configurations. Below are the commands to enter in the terminal:

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### Git Init
To start git version system, go to your desired project folder in terminal and enter 
```
git init
```
It'll initialize git for the folder and for all of its files and subfolders.

### Git Status
Status shows you what files are untracked, branch info, commit info, etc. Command:
```
git status
```
Example Output:
```
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

### Git add (Staging)
Staging is basically adding the untracked files in a queue to be tracked. Command
```
git add <filename>  # Specific files to be staged
git add .           # Stages all the changes of that folder and subfolders
```

### Git Commit
Commit is saving the version of the files(s) that has been changes/added/deleted. Command:
```
git commit -m "Commit Message"      # Commit staged changes
git commit -a -m "Commit Message"   # Commit all tracked changes, skiping staging
```

> ...To be Continued
### References
[Git Documentation](https://git-scm.com/doc)
[W3 Schools](https://www.w3schools.com/git/default.asp?remote=github) 