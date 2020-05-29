---
description: Staging And Committing Changes
---

# Committing Changes

We Stage our changes before committing changes. This is to avoid committing files that are not yet ready to be committed. 

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

