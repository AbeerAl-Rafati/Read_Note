# Git Tutorial


## Version Control
Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes.

## Git
Git is a Distributed Version Control (DVCS) which allows for multiple mirrored repositories, these data backups can be easily be placed on the server to replace any lost information.

Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.
Every single change applied to any file or directory is tracked by Git, Git will always detect file corruption or loss of information in transit.

Files in Git can reside in three main states: 
committed: Data is securely stored in a local database.
modified: File has been changed but not committed to the database.
staged: Flagged a file’s changed version to be committed in the next snapshot.


### Check Settings
Use this command:
*git config --list*

### Getting Help
Use one of these to call help:
* *git help command*

* *git command --help*

* *man git-command*

## Setting up a Git Repository
### Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

1. Switch to the target project’s directory (using *cd*  command).
2. Use the *git init* command, after creating a new subdirectory named .git.
3. To start tracking the represotry file, type this commands:
 *  *git add *.c*
 *  *git add LICENSE*
 *  *git commit -m “any message here”*

### Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:
git clone https://github.com/test 


### Local Repository Structure
The local Git repository has three components:
* Working Directory: The actual files reside here.
* Index: The area used for staging
* Head: Points to the most recent commit

### Saving Changes
**Tracked**
Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

**Untracked**
Untracked files were not in the last snapshot and do not currently reside in the staging area.


*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited*

### The Life Cycle of File Status
* After you edit a file, Git flags it as modified because of changes made after the previous commit.
* You stage the modified file.
* Then, you commit staged changes.


### Check File Status
Use *git status* command.


### Tracking and Staging a New File
* Track one file only by using the following format: *git add filename*.
* Track all files in a repository by using the following command: *git add **.

### Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message: *git commit -m “made change x,y,z”*.

### Committing All Changes
This command commits a snapshot of all modifications to tracked files in the working directory using this command: *git commit -a*.

### Pushing Changes
This command pushes changes from the local “master” branch to the remote repository named “origin”.
For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.

### Stashing Changes
When you are not ready to commit changes but do not want to lose them either, *git stash* is a great option. This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the *git stash apply* command to retrieve the hidden changes.

## Remote Repositories
### Cloned Repositories
As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

### Seeing Your Remotes
* Run  *git remote*  to show short names, such as “origin,” of all specified remote handles.
* Run  *git remote -v*  to show all the remote URLs next to their corresponding short names.
 
