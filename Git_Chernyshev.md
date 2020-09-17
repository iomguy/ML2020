
 ### *Summery for [Git Lecture](https://youtu.be/EPVwnG-n4B0)*

# P1: Git and GitHub
**Git** is a version control system. Git repositories stay on the computer's hard disc. Files are private.
**GitHub** is remote git repository. Repositories are stored in the cloud. GitHub storages are (mostly?) public, so everyone can see it.

Terms:
**working directory** = Files that you're currently working on (?)
**Index** = staging area
**Repository** = commit history
**Head** = Current position in the repository ('u r here')



## Basic Commands: 
1.  ### git add file.py
Starts tracking the version history of the file 
>How/why it happens?

...and adds it to the *staging area* which is like a purgatory.

2.  ### git commit file.py
Transfers files from the *staging area* to a Git repository for permanent storage. Makes the file **immutable**.
 - **Commit -m "hello?"**
Commit with a message.

>Committed files can be referenced either using **hash number**, or a shortcut:
Current repository version: **HEAD**
Previous: **HEAD~1** 
Before that: **HEAD~2**

3. ### git status
Shows what branch you're on, what is its state.

4.  ### git log
Shows the repository history: all the commits and all the commit messages.

5.  ### git diff
Shows difference between current repository and last commit. 
Also:
**git diff --staged**
Shows difference between  staging area and  last commit.
**git diff HEAD~1**
All the changes between 1 commits ago and now

6. ### git checkout HEAD file.py
Retrieves the last committed version of file.py

7. ### git reset --hard HEAD~1
Sets the HEAD at the previous committed version
>what's hard?

8. **git reflog**
Gives you the history of HEAD manipulations: where HEAD has been. If you lose some file.
>How can you **lose** a file? If the log is just a chronological tree w/ branches?!

## Branches

Separate branches for different projects.
There is the basic **master branch**.

Use to create a new branch:
**git checkout -b "branch_name**

Use to switch to a branch:
**git checkout master**

## Git -> GitHub

Commands:
**push**
To transfer the content to the server
**pull**
To synchronize local repository with the server

You can **fork** someone's repository (i.e. copy it),
then change it (using **push**) 
and then issue a **pull request** to the original page.
The repository's owner can either approve it and import the changes or not.

**Pull requests** are good because:
1. You can change repositories you don't have rights to change
2. You can show the changes that you've made.

After a version has been pushed by smb, you have to pull and **merge** them. You can't push anything before merging.

## Other stuff

- **.gitignore**
It's a text file that you put in the git folder with 1 program name/extetion (?) per line. Everything that matches its contents will be ignored by git (meaning it won't be tracked?)

- **A DOG: git log --all --decorate --oneline -graph**
Better use this for a readable log account

- **gitk**
User Interface to be used instead of **git log** (to see the repository contents)

- **git gui**
User interface for **adding** and **committing**
> GUI = graphic user interface


# P2: Unit Testing

*It's good to build  tests for the code. 
Write them in a separate file, starting with importing the original file. 
Then test it in **pytest***.
Among other things it helps determine wether the updates you made to the code were good or bad. Or to prevent already encountered bugs from happening again.

Types of tests:
- **Unit tests**
Paritcular part of the code does its thing.
- **Integration tests**
- **Non-Regression tests**
To make sure that a bug won't occur [again]

PyTest does **test coverage** showing what parts of the code were tested and which were left out. Coverage can be transfered to html which is useful.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYwMjEyNjgwOV19
-->