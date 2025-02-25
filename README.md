# Git-Commands

# Git Command Guide

This guide provides a summary of common Git commands organized by their usage, along with simple explanations and examples.

---

## 1. Starting a Working Area

- **`git clone`**  
  - **Purpose:** Makes a copy of a remote repository on your computer.
  - **Example:** `git clone https://github.com/user/repo.git`
  - **Explanation:** This command creates a new folder with all the files and history from the repository, allowing you to work on it locally.

- **`git init`**  
  - **Purpose:** Starts tracking a new or existing folder with Git.
  - **Example:** `git init`
  - **Explanation:** Initializes a Git repository in the current folder, enabling Git to track changes and save versions of files.

---

## 2. Working on the Current Change

- **`git add`**  
  - **Purpose:** Stages changes, marking files as ready to be saved in the next commit.
  - **Example:** `git add file.txt`
  - **Explanation:** Adds `file.txt` to the staging area, preparing it to be saved (committed) to the repository.

- **`git mv`**  
  - **Purpose:** Moves or renames a file and tells Git about it.
  - **Example:** `git mv oldname.txt newname.txt`
  - **Explanation:** Moves or renames `oldname.txt` to `newname.txt` and keeps Git aware of the change.

- **`git restore`**  
  - **Purpose:** Reverts changes in your working files.
  - **Example:** `git restore file.txt`
  - **Explanation:** Discards any changes in `file.txt` since the last commit, resetting it to the saved version.

- **`git rm`**  
  - **Purpose:** Deletes a file from the repository.
  - **Example:** `git rm file.txt`
  - **Explanation:** Removes `file.txt` from the working directory and stops Git from tracking it.

---

## 3. Examining the History and State

- **`git bisect`**  
  - **Purpose:** Finds the commit that caused a bug by testing different versions.
  - **Example:** `git bisect start`
  - **Explanation:** This command allows you to start marking good and bad commits, and Git helps narrow down which commit caused the issue.

- **`git diff`**  
  - **Purpose:** Shows differences between file versions.
  - **Example:** `git diff`
  - **Explanation:** Displays changes between the working directory and the last commit so you can see what you modified.

- **`git grep`**  
  - **Purpose:** Searches through your code for specific text.
  - **Example:** `git grep "function_name"`
  - **Explanation:** Finds all instances of `"function_name"` in your codebase.

- **`git log`**  
  - **Purpose:** Shows the history of commits in the repository.
  - **Example:** `git log`
  - **Explanation:** Lists all past commits with details like the author, date, and message so you can review the changes.

- **`git show`**  
  - **Purpose:** Shows details about a specific commit.
  - **Example:** `git show abc1234`
  - **Explanation:** Displays what was changed in a specific commit (`abc1234`), along with other details.

- **`git status`**  
  - **Purpose:** Shows the status of files in your working directory and staging area.
  - **Example:** `git status`
  - **Explanation:** Tells you which files have changes and whether they’re staged, unstaged, or untracked.

---

## 4. Growing, Marking, and Tweaking Your Common History

- **`git branch`**  
  - **Purpose:** Manages branches in your project.
  - **Example:** `git branch new-feature`
  - **Explanation:** Creates a new branch called `new-feature` where you can make changes without affecting the main branch.

- **`git commit`**  
  - **Purpose:** Saves staged changes to the repository.
  - **Example:** `git commit -m "Add new feature"`
  - **Explanation:** Takes a snapshot of your staged changes and saves it as a commit with a message describing the changes.

- **`git merge`**  
  - **Purpose:** Combines changes from one branch into another.
  - **Example:** `git merge new-feature`
  - **Explanation:** Merges the `new-feature` branch into your current branch, combining the changes.

- **`git rebase`**  
  - **Purpose:** Moves or replays commits from one branch onto another.
  - **Example:** `git rebase main`
  - **Explanation:** Re-applies commits on top of another branch, often used to keep a clean commit history.

- **`git reset`**  
  - **Purpose:** Unstages or undoes commits by moving the `HEAD` pointer.
  - **Example:** `git reset HEAD~1`
  - **Explanation:** Moves the `HEAD` back by one commit, effectively undoing the last commit without deleting your files.

- **`git switch`**  
  - **Purpose:** Switches to another branch.
  - **Example:** `git switch new-feature`
  - **Explanation:** Changes the current branch to `new-feature` so you can start working on it.

- **`git tag`**  
  - **Purpose:** Labels a specific commit, often for marking releases.
  - **Example:** `git tag v1.0`
  - **Explanation:** Creates a tag called `v1.0` at the current commit, often used to label versions like releases.

---

## 5. Collaborating with Others

- **`git fetch`**  
  - **Purpose:** Gets changes from a remote repository without applying them to your branch.
  - **Example:** `git fetch origin`
  - **Explanation:** Downloads new data from the remote but doesn’t merge it, so you can review it before applying.

- **`git pull`**  
  - **Purpose:** Gets and applies changes from a remote repository.
  - **Example:** `git pull origin main`
  - **Explanation:** Fetches and merges changes from the `main` branch on the remote repository into your current branch.

- **`git push`**  
  - **Purpose:** Sends your commits to a remote repository.
  - **Example:** `git push origin main`
  - **Explanation:** Uploads your changes to the `main` branch on the remote repository, making them available to others.

---

Git command

git login by command
* git config --global user.name "TrickAndTarck" 
* git config --global user.email "xyz@gmail.com"
for the conform 
*git config --global user.name
or
whoami

print working directory
*pwd

showing the working of keywords
*git help

branch switching
*git switch <branch name> 


1) if we want to push code on new  repo->

a) git init  (create empty git repository)
b) git status (for checking files)
c) git add .
d) git commit -m "project commit"
e) git status
d) git remote add origin https://github.com/TrickAndTrack/a.git
f) git push -u origin <master/main/branchname>

2) if we want to take a pull in new pc/new folder->

a) git init
b) git status (Cross Check which files are in modifed  )
c) git add .
d) git commit -m "project commit"
e) git remote add origin <git repo url>
f) git remote -v
g) git push -u origin <master/main/branchname>


3) how to pull requests genrate
a) git switch <branch name> 
b) git add .
c) git commit -m "<Git message>"
d) git push


This guide provides a quick reference for common Git commands, their purposes, and usage examples. Keep this on hand as you work with Git to manage your projects!
