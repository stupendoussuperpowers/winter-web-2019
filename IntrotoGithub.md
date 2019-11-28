# Introduction to Github
 Git is a free and open-source version control system, that helps you keep track of changes to files in a filesystem/repository over time. It has been an industry        standard for a while now. Git comes with the git-shell which has a set of nifty commands that can help you do all sorts of things on your repositories.

 Github is a service that hosts your repositories online and lets you collaborate with others through it. You can use Github through the browser or the git-shell on your pc. Github also helps you collaborate with people around the globe! 

 Collaborators from different regions around the world, can work on same projects, with the help of Github, as it helps accessing code by other programmers, really easy!

## How to install github?
**Windows**: https://hackernoon.com/install-git-on-windows-9acf2a1944f0

**Linux**: For Debian and Ubuntu - ```sudo apt-get install git```  
and check git version using - ```git --version```

**MacOS**: https://hackernoon.com/install-git-on-mac-a884f0c9d32c

# Git Cheat Sheet
## Create Repositories
To clone an existing repository:

```$gitdonessh://user@domain.com/repo.git``` 

To create a new local repository: 

 ```$ git init``` 

## Configure Tooling
#### Configure user information for all local repositories

Sets the name you want attached to your commit transactions:

 ```$ git config --global user.name "[name]"``` 

Sets the email you want attached to your commit transactions:

  ```$ git config --global user.email "[email address]"``` 

Enables helpful colorisation of the command line output:

  ```$ git config --global color ui.auto ``` 

## Make Changes
#### Review edits and craft a commit transaction
 Lists all the modified files to be committed:

 ``` $ git status```

Shows file differences not yet staged:

 ``` $ git diff``` 

Snapshots the file preparation for versioning:

 ``` $ git add[file]``` 

Shows file differences between staging and the last final version:

 ``` $ git staged  --staged```

Unstages the file, but preserves its contents: 

 ``` $ git reset [file]```

Records file snapshots permanently in version history:

 ``` $ git commit - m "[descriptive message]"```

## Group Changes
#### Name a series of commits and combine completed effort 
Lists all the local branches in the current repository:

 ``` $ git branch ``` 

Creates new branch:

 ``` $ git branch [branch name]```

Switches to specified branch and updates the working directory:

 ``` $ git checkout [branchname]```

Combines specified branch's history into the current branch:

 ``` $ git merge [branch name]```

Deletes the specified branch:

 ``` $ git branch -d [branch name]```

## Refactor Filenames
#### Relocate and remove versioned files 
Deletes the file from the working directory and stages the deletion: 

 ``` $ git rm [file]``` 

Removes the file from the version control but preserves the file locally:

 ``` $ git rm -- cached [file]```

Changes the file name and prepares for commit:

 ``` $ git mv [file-original] [file-renamed]``` 

## Supress Tracking
#### Exclude temporary files and paths
 A  text file named ``.gitignore`` supressess accidental versioning of files and paths matching the specified patterns:

 ``` *. log build/temp- *```

Lists all ignored files in this project:

  ```$ git ls-files --other --ignored --exclude-standard```  

## Save Fragments
#### Shelve and restore incomplete changes

Temporarily stores all the modified tracked files:

 ```$ git stash```

 Restores the most recently stashed files:

 ```$ git stash pop```

 Lists all stashed:

 ```$ git stash list ```

 Discards the most recently stashed changeset: 

 ```$ git stash drop ```

## Review History
#### Browse and inspect the evolution of project files 
 Lists version history for current branch:

 ```$ git log```

 Lists version history for a file, including renames:

 ```$ git log --follow[file]``` 

 Shows content differences between two branches:

 ```$ git diff [first-branch] . . . [second branch]```

 Outputs metadata and content changes of the specified commit: 

 ```$ git show [commit]```

## Redo Commits
#### Erase mistakes and craft replacement history
 Undoes all commits after ``[commit]``, preserving changes locally:

  ```$ git reset``` 

 Discards all hsitory and changes back to the specified commit:

 ```$ git reset --hard [commit]``` 

## Synchronize Changes
#### Register a repository bookmark and exchange version history
 Downloads all history from the repository bookmark:

 ```$ git fetch [bookmark]```

 Combines bookmark's branch into the curent local branch:

 ```$ git merge [bookmark]/[branch]```

 Uploads all local branch commits to GitHub:

 ```$ git push [alias] [branch]```

 Downloads bookmark history and incorporates changes:

 ```$ git pull``` 

## Tutorials to get you started 

- https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners
- https://git-scm.com/docs/gittutorial
- https://medium.com/@abhishekj/an-intro-to-git-and-github-1a0e2c7e3a2f