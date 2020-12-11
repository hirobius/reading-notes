# day_3

###### [day_1](day_1.md)
###### [day_2](day_2.md)
###### [day_3](day_3.md)
###### [day_4](day_4.md)
###### [day_5](day_5.md)
###### [day_6](day_6.md)
###### [day_7](day_7.md)
###### [day_8](day_8.md)
###### [day_9](day_9.md)
###### [day_10](day_10.md)


Git: Version Control
GitHub: Online Code Storage

git status
git add
git commit
git push

***Small, frequent commits is the name of the game!***

### Version Control

In order to explain Git, we have to first explain various aspects of Version Control.

Version Control Systems (VCS) are like a dynamic "history" record that you can revert your work back to, keep track edits including who edited what and when.

These can be stored locally as a **Local** VCS on your Hard Drive. 

The need to be able to collaborate led to a Centralized VCS (CVCS) which is accessible by various clients all at once.

But in case things broke or became corrupted, there was the advent of the Distributed VCS (DVCS) which permitted "mirrored" iterations of one repository that could easily repair or replace any mishaps or lost info. This also enabled more dynamic collaboration methods and workflows.


### So What is Git?

Git is a DVCS and saves "snapshots" of your work every time you save.

Git relies on local information in order to speed up the fetching of information (doing so from a remote server is slower) and you are also able to continue working while offline :)

Git is very smart and tracks every little detail, good or bad, which makes it difficult for you to actually lose work!


### Git Stages

Committed: Data is securely stored in a local database.

Modified: File has been changed but not "committed" to the database.

Staged: A file's changed version is ready to be committed to the next snapshot.

History: Git was created by the founder of Linux kernel, dude named Linus Torvalds, and is now one of the most widely used VCS in the world.



### Customization

Git comes with a built in GUI, but you can download additional GUI clients [HERE](https://git-scm.com/downloads/guis).

The built-in ```git config``` is pretty much the settings directory which allows the configuration of variables that control aspects of Git’s operation and look.


**To set your Identity *(username and email address)* for every Git commit, type the following into the command line:**

``` 
git config --global user.name "Jane Smith"
git config --global user.email "example@email.com"
```

**To confirm everything's working, type the following into the command line**

```
git config --global user.name (should return Jane Smith)

git config --global user.email (should return example@email.com)
```

By using ```--global``` you are doing system-wide changes, so if you only want to affect the contents of the current directory then don't use it.


### Default Text Editor
By using ```git config --global core.editor (editor name here)``` you can change the default Text editor. For some editors there are different steps to accomplish this.


### Check Settings
To check settings, use the ```git config --list``` command.

### Getting Help
```
git help (command here no parentheses)
git (command here no parentheses) --help
man git-(command here no parentheses)
```

## Setting up a Git Repository

### Importing

To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

**1** Switch to the Target Project's Directory:
```cd test (cd = change directory)```

**2** Use the git init command
```git init```

*Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.*

**3** To start tracking these repository files, perform an initial commit by typing the following:
```git add *.c```
```git add LICENSE```
```git commit -m “any message here”```


## Cloning

This will duplicate your all versions of all files in the project named "test":
```git clone https://github.com/test```

If you want to use your own name, use:
```git clone https://github.com/test mydirectory```

The command above makes a copy of the target repository in a directory named “mydirectory.”


### Workflow

**1** Working Directory: Where the files live
**2** Index: Staging Area
**3** Head: Points to the most recent commit


### Saving Changes

**Tracked** Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
**Untracked** These were not in the last snapshot and do not currently reside in the staging area.


### The Life Cycle of File Status

First you edit, then the file is flagged as "modified", then you stage, then you commit the staged changes. Rinse and repeat.

To determine the state of files, utilize the ```git status``` command. This will indicate which branch you're on and states (haven't covered that yet).


## Tracking and staging a new file

***After using the folowing commands, files are tracked and staged for committing***

### Single File

```git add filename``` to track one file

### All Files

```git add *``` to track all files in a repository


## Committing a file

```git commit -m “made change x,y,z”``` to commit a file or multiples and include a commit message which will apply to all being committed at this time.

## Committing all changes
```git commit -a``` to commit a snapshot of all modifications to tracked files in the working directory.

## Pushing changes

Next you would PUSH all changes to the remote repository with the command ```git push origin master``` *(origin being where you cloned from and master being your local repository. You can actually change these names if you want.)* 

## Stashing changes

When you are not ready to commit changes but want to save your work, use the command ```git stash``` to remove and hide your changes then ```git stash apply``` to retrieve

## Remote Repositories

### Seeing your Remotes

```git remote``` command to view the short names of all specified remote handles
```git remote -v``` to view all the short names next to their remote URLs
