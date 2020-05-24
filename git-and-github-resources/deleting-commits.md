---
description: Deleting Commits Made
---

# Deleting Commits

Three different types:

Checkout commit - To view commits.  
         Revert commit - To remove a particular commit in time.  
         Reset commit - To go back in time and delete all other commits.

### **Reverting Commits**

```text
git log --oneline
git checkout commitcode        # commitcode = code of commit
git checkout master            # To return back to present.
git revert commitcode
```

**Note** : git revert does not delete the commit, it reverts the commit by creating a new commit that removes all the changes. **Note** : when reverting, it asks for your message. To escape this screen, press shift and **:wq**

### **Resetting Commits**

```text
git reset commitcode            # Resets back to the needed commit. But, retains the code if you still want to use it.
git reset commitcode --hard     # Resets back to the needed commit. Deletes all the code and there is no reverting back.
```

