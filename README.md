# Git & GitHub Commands Notes
  
## 1. Git Configuration

### Check Git Version

```bash
git --version
```

### Set Username

```bash
git config --global user.name "Your Name"
```

### Set Email

```bash
git config --global user.email "your@email.com"
```

### Check Configuration

```bash
git config --list
```

---

# 2. Initialize Repository

### Create Git Repository

```bash
git init
```

### Check Status

```bash
git status
```

---

# 3. Staging Files

### Add Single File

```bash
git add filename.cpp
```

### Add All Files

```bash
git add .
```

---

# 4. Commit Changes

### Commit Changes

```bash
git commit -m "Initial commit"
```

### View Commit History

```bash
git log
```

### Compact Commit History

```bash
git log --oneline
```

---

# 5. Branching

### View Branches

```bash
git branch
```

### Create New Branch

```bash
git branch work
```

### Switch Branch

```bash
git checkout work
```

### Create & Switch Together

```bash
git checkout -b work
```

### Modern Way

```bash
git switch work
```

### Create & Switch (Modern)

```bash
git switch -c work
```

---

# 6. Merging

### Move to Main Branch

```bash
git switch main
```

### Merge Work Branch

```bash
git merge work
```

---

# 7. Delete Branch

### Delete Branch After Merge

```bash
git branch -d work
```

### Force Delete Branch

```bash
git branch -D work
```

---

# 8. GitHub Connection

### Connect Repository

```bash
git remote add origin <repository-url>
```

### Check Remote

```bash
git remote -v
```

---

# 9. Push Code

### First Push

```bash
git push -u origin main
```

### Normal Push

```bash
git push
```

### Push Specific Branch

```bash
git push origin work
```

---

# 10. Pull Code

### Download Latest Changes

```bash
git pull
```

### Pull Specific Branch

```bash
git pull origin main
```

---

# 11. Clone Repository

```bash
git clone <repository-url>
```

---

# 12. Tags (Versioning)

### Create Tag

```bash
git tag v1.0.0
```

### Create Annotated Tag

```bash
git tag -a v1.0.0 -m "First Release"
```

### View Tags

```bash
git tag
```

### Push Single Tag

```bash
git push origin v1.0.0
```

### Push All Tags

```bash
git push --tags
```

---

# 13. Undo Changes

### Remove File From Staging

```bash
git restore --staged filename.cpp
```

### Discard Local Changes

```bash
git restore filename.cpp
```

### Undo Last Commit (Keep Changes)

```bash
git reset --soft HEAD~1
```

### Undo Last Commit (Remove Changes)

```bash
git reset --hard HEAD~1
```

---

# 14. Useful Commands

### Show Differences

```bash
git diff
```

### Show Staged Differences

```bash
git diff --staged
```

### Show Current Branch

```bash
git branch --show-current
```

### View Commit Graph

```bash
git log --oneline --graph --all
```
---
# 15. Stash Commands

### Save Current Changes

```bash
git stash
```

### View Stash List

```bash
git stash list
```

### Apply Latest Stash

```bash
git stash apply
```

### Apply and Remove Stash

```bash
git stash pop
```

### Delete Stash

```bash
git stash drop
```

### Clear All Stashes

```bash
git stash clear
```

---

# 16. Rebase Commands

### Rebase Current Branch

```bash
git rebase main
```

### Interactive Rebase

```bash
git rebase -i HEAD~5
```

### Continue Rebase

```bash
git rebase --continue
```

### Abort Rebase

```bash
git rebase --abort
```

---

# 17. Fetch Commands

### Fetch Latest Changes

```bash
git fetch
```

### Fetch All Remotes

```bash
git fetch --all
```

---

# 18. File Operations

### Remove File

```bash
git rm file.txt
```

### Rename File

```bash
git mv old.txt new.txt
```

---

# 19. Remote Commands

### List Remotes

```bash
git remote
```

### Detailed Remote Information

```bash
git remote show origin
```

### Remove Remote

```bash
git remote remove origin
```

### Rename Remote

```bash
git remote rename origin upstream
```

---

# 20. Reset Commands

### Unstage File

```bash
git reset file.txt
```

### Soft Reset

```bash
git reset --soft HEAD~1
```

### Mixed Reset

```bash
git reset --mixed HEAD~1
```

### Hard Reset

```bash
git reset --hard HEAD~1
```

---

# 21. Cherry Pick

### Apply Specific Commit

```bash
git cherry-pick <commit-hash>
```

---

# 22. Clean Repository

### Preview Deletion

```bash
git clean -n
```

### Delete Untracked Files

```bash
git clean -f
```

### Delete Untracked Files & Folders

```bash
git clean -fd
```

---

# 23. Inspection Commands

### Show Commit Details

```bash
git show
```

### Show Specific Commit

```bash
git show <commit-hash>
```

### View Reference Log

```bash
git reflog
```

### Show File History

```bash
git blame file.cpp
```

---

# 24. Search Commands

### Search Text in Repository

```bash
git grep "keyword"
```

---

# 25. Submodule Commands

### Add Submodule

```bash
git submodule add <repository-url>
```

### Initialize Submodule

```bash
git submodule init
```

### Update Submodule

```bash
git submodule update
```

---

# 26. Archive Commands

### Create ZIP Archive

```bash
git archive --format=zip HEAD -o project.zip
```

---

# 27. Git Help Commands

### General Help

```bash
git help
```

### List All Commands

```bash
git help -a
```

### Help for Specific Command

```bash
git help commit
```

### Branch Help

```bash
git help branch
```

### Merge Help

```bash
git help merge
```

### Push Help

```bash
git help push
```

### Pull Help

```bash
git help pull
```

---

# 28. Advanced Log Commands

### Compact History

```bash
git log --oneline
```

### Graph View

```bash
git log --oneline --graph --all
```

### Last 5 Commits

```bash
git log -5
```

### Commit Statistics

```bash
git log --stat
```

---

# 29. Useful Daily Commands

### Current Branch

```bash
git branch --show-current
```

### Repository Status

```bash
git status
```

### Compare Changes

```bash
git diff
```

### Compare Staged Changes

```bash
git diff --staged
```

### Latest Commit Hash

```bash
git rev-parse HEAD
```

---

# 30. Professional Release Workflow

```bash
git add .

git commit -m "Final update"

git push

git tag -a v1.0.0 -m "First Stable Release"

git push origin v1.0.0
```

---

# Daily Workflow

```bash
git status

git add .

git commit -m "Added new feature"

git push
```

---

# New Feature Workflow

```bash
git switch -c feature-name

# Do work

git add .
git commit -m "Added feature"

git switch main

git merge feature-name

git push

git branch -d feature-name
```


---

## Author

**Yuvraj Singh**

* C++ Developer
* DSA & LeetCode Enthusiast
* GitHub: https://github.com/your-username
* LeetCode: https://leetcode.com/u/Yuvrajsinghz/

---

⭐ If these notes helped you, consider starring the repository and sharing it with others.

**Happy Coding! 🚀**
