# **Revisions and the Cloud**

## **Version control**

Version Control allows you to revisit versions of a file or set of files by recording changes. With version control you can return to a file or make changes to a previous version and compare those changes. Using a VCS, mistakes can be corrected.

### **3 Types of Version Control Systems**
- LVCS: Local Version Control
    Database on your Hard Drive.
- CVCS: Centralized Version Control
    Single Server that stores file versions and changes to be accessed by clients. Used for collaboration of a team.
- DVCS: Distributed Version Control
    VCS where complete codebase is mirrored on all dev's computers. Gives dev's the ability to work offline.

## **What is Git?**

Git is an open sourced DVCS designed for tracking changes in source code during software development. 

### ***Snapshots***

Snapshots are to repositories, as a screenshot would be for videos. Every saved change, aka commit, Git creates a snapshot and stores reference.

### ***Local Operations***

Git depends on local operations since most important info can be found on your local disk instead of having to fetch history from server even when offline or on a Virtual Private Network.

### ***Tracking Changes***

All changes to any file or directory is tracked by Git. Git detects file corruption/mistakes and info lost in transit.

### ***Loss of Data***

Git was designed to minimize possibility of irreversible damage to files, like in the case of an accident.

### ***States***

Files in Git reside in 3 main states.

*Committed*
Data is securely stored in local database
*Modified*
File has been changed but not commited
*Staged*
Flagged/highlighted a file's changed version to be commited in next Snapshot

## **Working with Git**

There are two types of commands used in Git.
    -*Bash commands*
    Commands native to bash/shell. Allow you to navigate around your computer, explore directories, create and modify files and directories etc. (ex: ls, cd, mkdir, etc.)
    -*Git commands*
    Specific to Git and only available if git is installed. Git commands will always start with git prefix (ex: git status, git clone etc.)

## **What is GitHub?**

GitHub itself is a Git repository hosting service but adds plenty of its own features. Git being a command line tool, GitHub provides the web-based GUI. It also provides access control and collaboration features.

## **Local vs. Remote**

You can git branch -a to list all branches (local and remote) then choose branch name from list (just remove remotes/ from remote branch name. Example: git diff master origin/master (where "master" is local master branch and "origin/master" is a remote namely origin and master branch.)

## **Cloning Repositories**

To clone a new repository from GitHub to your local computer, simply:
    1. Repository page
    2. Click green button "Clone/download"
    3. Copy URL for repository
    4. From Local Machine, open bash shell and change current directory to location where you want to clone your repository
    -Here we are using a bash command - cd (change directory)
    5. Once you picked the directory you want your repository you can type *git clone **https://github.com/URL-TO-REPO-HERE***
The *git clone* command copies your repository from GitHub to local computer.
-Remember: this is a git specific command.
    6. When you run *git clone repo-path-here*, you should see an output like
    
    EX: cloning into 'test-repo'...
        remote: counting objects: 5, done.
        remote: compressing objects: 100% (4/4), done.
        remote: Total 5 (delta 0) reused 0 (delta 0) pack-reused 0
        unpacking objects: 100% (5/5), done.
        Checking connectivity... done.

## **What does ACP stand for?**

    - A: Add (Tracking and Staging a new file)

Track one file only by using:
*'git add filename'*
Track all files in a repo by using:
*'git add *'*
Afterwards you can check info by *'git status'*

    - C: Commit (Saving Changes)
You can do this by typing *'git commit -m "changemade" '*

    - P: Push (Linking changes between local and remote)

Ex: *'git push origin master'*

## **Deployment!**

Once all of your files in your repository are to your satisfication, now you are ready to Deploy (publish) your site!

