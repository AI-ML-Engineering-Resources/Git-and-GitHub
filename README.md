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
Example Outout:
```
Initialized empty Git repository in C:/Personal-Projects/test/.git/
```
It'll initialize git for the folder and for all of its files and subfolders.

### Git Status
Status shows you what files are untracked, branch info, commit info, etc. Command:
```
git status
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
git commit -m "Commit Message"           # Commits staged changes
git commit -a -m "Commit Message"        # Commits all modified/deleted changes, not new files; skips staging
git commit --allow-empty -m "Message"    # Empty commit, no change added
```

### Git Stash
Stashing is like creating a temporary storage for the changes (like a clipboard). It saves the temporary changes and returns to the last commited version for the repository. Commands:
```
git stash                       # Stashing tracked changes
git stash -u                    # Stashing tracked/untracked changes
git stash push -m "Message"     # Stash with message
git stash list                  # List all stashes
git stash pop                   # Reapplies latest stash changes and takes off the stash list
git stash apply                 # Reapplies latest stash changes but keeps the stash in the list
git stash apply stash@{n}       # Reapplies specific stash
```

### Git Log
Git log shows the history. Command:
```
git log                 
git log --oneline       # Shorter history
git log --stat          # Shows filenames which changed with history as well 
```
To end the log mode, just press q in the terminal.

### Git diff
See tracked/untracked changes using diff. Commands:
```
git diff            # Unstaged changes
git diff -staged    # Staged changes
```
### Git Branch
Branching is like creating a seperate workplace for the project where you can create new versions and its changes without affecting the main section. Commands:
```
git branch                  # Lists all branches
git branch <branch name>    # Create a new branch
git checkout <branch name>  # Changes your workplace to the specific branch
```
> ...To be Continued
### References
[Git Documentation](https://git-scm.com/doc)
[W3 Schools](https://www.w3schools.com/git/default.asp?remote=github) 