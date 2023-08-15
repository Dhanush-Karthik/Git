# Git-Basics
Basic commands and concepts of Git

## Clone a remote repository

To clone a remote git repository use the following command:

`git clone <Https/SSH repository link>`

## Get the status of the local repository

To get the status of the local repository use the following command:

`git status`

## Staging area

The staging area, also commonly referred to as the "index," is an intermediate step in the Git version control system that allows you to prepare and organize changes before committing them to the repository. It acts as a buffer between your working directory (where you make edits) and the repository's history (where your changes are permanently recorded).

**Working Directory:** This is where you create, modify, and delete files as you work on your project.

**Staging Area:** After you make changes to your files in the working directory, you can use the git add command to stage these changes. Staging is the process of selecting specific changes to include in the next commit. When you stage changes, Git takes a snapshot of the current state of the modified files and places them in the staging area.

**Commit:** Once your changes are staged in the staging area, you can create a commit using the git commit command. A commit is a permanent record of the changes you've staged. It includes a snapshot of the staged changes, a unique identifier (SHA-1 hash), a timestamp, and the author's information. Committing effectively saves your changes to the repository's history.

## Tell git to track your new file

To tell git to track your new file use the command:

`git add <file name>`

The `git add` command moves changes from the working directory to the Git staging area. The staging area is where you prepare a snapshot of a set of changes before committing them to the official history.

`git add .` adds all the changes to the staging area.


![Alt text](https://wac-cdn.atlassian.com/dam/jcr%3Adbf0c59f-848d-4814-bfd5-6b190a092963/03.svg?cdnVersion%3D1162)

## Commit changes to git

You can commit the changes to your local repository using the command:

`git commit -m "your commit message"`

The git commit takes the staged snapshot and commits it to the project history.

Up until this point, everything you have done is on your local system and invisible to your Remote repository until you push those changes.

## Pushing your changes to remote repository

You can push your changes to remote repository using the command:

`git push origin branch_name`

**origin:** Refers to the remote repository.
**branch:** Refers to the branch to which you want to push your changes