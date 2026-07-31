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
