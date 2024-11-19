# GitHub Commands Cheat Sheet

This document contains commonly used Git and GitHub commands that developers frequently use.

---

## **Configuration**
### Set User Information
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

### View Configuration
```bash
git config --list
```

---

## **Repository Management**
### Initialize a Git Repository
```bash
git init
```

### Clone a Repository
```bash
git clone <repository-url>
```

---

## **Staging and Committing**
### Check Repository Status
```bash
git status
```

### Add Changes to Staging Area
```bash
git add <file>           # Add specific file
git add .                # Add all files
```

### Commit Changes
```bash
git commit -m "Your commit message"
```

---

## **Branch Management**
### List Branches
```bash
git branch               # Local branches
git branch -r            # Remote branches
git branch -a            # All branches
```

### Create a New Branch
```bash
git branch <branch-name>
```

### Switch Branch
```bash
git checkout <branch-name>
```

### Create and Switch to a New Branch
```bash
git checkout -b <branch-name>
```

### Delete a Branch
```bash
git branch -d <branch-name>      # Delete local branch
git push origin --delete <branch-name> # Delete remote branch
```

---

## **Remote Repository**
### Add Remote Repository
```bash
git remote add origin <repository-url>
```

### View Remote URLs
```bash
git remote -v
```

### Push Changes to Remote Repository
```bash
git push origin <branch-name>
```

### Pull Changes from Remote Repository
```bash
git pull origin <branch-name>
```

---

## **Merging and Rebasing**
### Merge a Branch
```bash
git merge <branch-name>
```

### Rebase Branch
```bash
git rebase <branch-name>
```

---

## **Stash Changes**
### Save Uncommitted Changes
```bash
git stash
```

### Apply Stashed Changes
```bash
git stash apply
```

### List Stashes
```bash
git stash list
```

### Drop a Stash
```bash
git stash drop
```

---

## **Logs and History**
### View Commit Logs
```bash
git log
git log --oneline       # Shortened log
git log --graph         # Show branch structure
```

---

## **Undo Changes**
### Unstage a File
```bash
git reset <file>
```

### Undo Last Commit (Keep Changes)
```bash
git reset --soft HEAD~1
```

### Undo Last Commit (Discard Changes)
```bash
git reset --hard HEAD~1
```

---

## **Tagging**
### Create a Tag
```bash
git tag <tag-name>
```

### Push Tag to Remote
```bash
git push origin <tag-name>
```

---

## **GitHub-Specific**
### Fork a Repository
1. Visit the repository on GitHub.
2. Click the **Fork** button.

### Create a Pull Request
1. Push changes to a feature branch.
2. Go to the repository on GitHub.
3. Click **Pull Requests > New Pull Request**.
4. Select the feature branch and submit.

---

## **Tips**
### Set Up SSH
```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
Add the SSH key to your GitHub account.

---

### Helpful Links
- [Git Documentation](https://git-scm.com/doc)
- [GitHub CLI](https://cli.github.com/)

