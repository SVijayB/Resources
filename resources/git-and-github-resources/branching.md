---
description: 'Creating, using and deleting Branches using Git'
---

# Branching

### **Creating a branch**

```text
git branch branchname
git checkout -b branchname      # This creates a branch and automatically opens up the branch.
```

### **Checking out all the branches**

```text
git branch -a
```

### **Switching to a branch** 

```text
git checkout branchname
```

### **Merging branches** 

```text
git checkout master         # Note : Go to the branch you want to merge into.
git merge branchname        # Enter name of the branch you want to merge.
```

### **Deleting a branch**

```text
git checkout master          # Note : Go to a different branch than the one you are deleting.
git branch -d branchname     # Works only if you have merged the branch.
git branch -D branchname     # Works even if you haven't merged the branch.
```

### **Pushing a branch to GitHub**

```text
git checkout -b branchname    # Creates a new branch
git push origin branchname    # Creates branch in GitHub and pushes all changes to that branch
```

Now compare changes and create pull request on GitHub.

### Updating the feature branch

After merging pull requests from various branches, our master branch might be a few commits ahead of our feature branch. In order to even the feature and master branch, we have to merge changes. To do this, use :

```text
git checkout branchname     # The feature branch you want to update
git merge master            # Updates the branch
git push                    # Updates the feature branch on the remote repository
```

### **Deleting branch history**

```text
git remote prune origin
```

**Note** : Before you create a new branch, always make sure you have the latest version of master on your local repository. To do this, use : `git pull origin master`

