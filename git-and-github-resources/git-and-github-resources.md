---
description: A simple and easy to understand guide towards getting started with GitHub
---

# Getting Started

## Getting Started with Git And GitHub

![GitHub](https://i.ibb.co/cXW10PW/Logo.jpg)

## What is GitHub?

At its heart, GitHub is a collaboration platform.  
 From software to legal documents, you can count on GitHub to help you do your best work with the collaboration and security tools your team needs. With GitHub, you can keep projects completely private, invite the world to collaborate, and streamline every step of your project.

## What is VCS?

GitHub uses Git, the most popular open source version control software, to track every contribution and contributor to your project--so you know exactly where every line of code came from.

## What you are going to learn

* Committing 
* Deleting Changes
* Branching

## Simple cmd commands you might need :

```text
cd ..                        # Goes up a folder
cd directoryname             # Enters the folder
mkdir foldername             # Creates a folder
echo >> filename.format      # Creates a file
notepad filename.format      # Opens the file in notepad
rm filename.format           # Deletes the file
rmdir foldername             # Deletes the folder
```

### **Moving a file to the staging area\(Before committing\)**

```text
git add filename.format
git add .                         # Adds all the files in directory
git rm --cached filename.format   # Removes the file from staging.
```

### **Committing changes**

```text
git commit -m "Enter descriptive information"
```

### **Viewing commit history**

```text
git log
git log --oneline             # Abstract view of commits
```

### Reverting changes

Three different types:

Checkout commit - To view commit.  
         Revert commit - To remove a particular commit in time.  
         Reset commit - To go back in time and delete all other commits.  


**Revert Commit**

```text
git log --oneline
git checkout commitcode        # commitcode = code of commit
git checkout master            # To return back to present.
git revert commitcode
```

**Note** : git revert does not delete the commit, it reverts the commit by creating a new commit that removes all the changes. **Note** : when reverting, it asks for your message. To escape this screen, press shift and **:wq**

### **Resetting changes**

```text
git reset commitcode            # Resets back to the needed commit. But, retains the code if you still want to use it.
git reset commitcode --hard     # Resets back to the needed commit. Deletes all the code and there is no reverting back.
```

### Branching

**Creating a branch:**

```text
git branch branchname
git checkout -b branchname      # This creates a branch and automatically opens up the branch.
```

**Checking out all the branches:**

```text
git branch -a
```

**Switching to branch :**

```text
git checkout branchname
```

**Merging branches :**

```text
git checkout master         # Note : Go to the branch you want to merge into.
git merge branchname        # Enter name of the branch you want to merge.
```

**Deleting a branch:**

```text
git checkout master          # Note : Go to a different branch than the one you are deleting.
git branch -d branchname     # Works only if you have merged the branch.
git branch -D branchname     # Works even if you haven't merged the branch.
```

**Pushing a branch to GitHub:**

```text
git checkout -b branchname    # Creates a new branch
git push origin branchname    # Creates branch in GitHub and pushes all changes to that branch
```

Now compare changes and create pull request on GitHub.

**Note** : Before you create a new branch, always make sure you have the latest version of master on your local repo. To do this, use : `git pull origin master`

### **Deleting branch history**

```text
git remote prune origin
```

Sometimes, after creating a release, you have to update the tags on local repo. To do so, use : `git fetch --tags -f`

