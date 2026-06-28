# 🛠️ Complete Command Reference

All user and developer commands for Hacker_Kal_AI.

## 📥 Cloning and Setup

### Clone Repository

```bash
# HTTPS
git clone https://github.com/Shanto008SB/Hacker_Kal_AI.git

# SSH
git clone git@github.com:Shanto008SB/Hacker_Kal_AI.git

# GitHub CLI
gh repo clone Shanto008SB/Hacker_Kal_AI
```

### Enter Directory

```bash
cd Hacker_Kal_AI
```

## 🚀 Running Local Server

### Option 1: Live Server (VS Code) - Recommended

```bash
# Install Live Server extension
# Right-click index.html → "Open with Live Server"
# Opens at http://localhost:5500
```

### Option 2: Python

```bash
# Python 3.x
python -m http.server 8000

# Python 2.x
python -m SimpleHTTPServer 8000

# Browser: http://localhost:8000
```

### Option 3: Node.js

```bash
# Install http-server
npm install -g http-server

# Run
http-server

# Browser: http://localhost:8080
```

### Option 4: PHP

```bash
php -S localhost:8000
# Browser: http://localhost:8000
```

## 🔧 Git Commands

### Branch Management

```bash
# Create new branch
git checkout -b feature/NewFeature

# List branches
git branch -a

# Delete branch
git branch -d feature/NewFeature
git branch -D feature/NewFeature  # Force delete
```

### Commit Changes

```bash
# Add all files
git add .

# Add specific file
git add index.html

# View changes
git status

# Commit
git commit -m "feat: Add new feature"

# Detailed commit
git commit -m "feat: Add new feature
- Added feature X
- Added feature Y"
```

### Push and Pull

```bash
# Push to GitHub
git push origin main

# Push branch
git push origin feature/NewFeature

# Pull from GitHub
git pull origin main

# Force Push (use carefully!)
git push origin main --force
```

### Logs and History

```bash
# View commits
git log

# Pretty log
git log --oneline --graph --all

# File history
git log -p index.html

# Recent changes
git diff

# Specific file diff
git diff index.html
```

### Tags

```bash
# Create tag
git tag v1.0.0

# Tag with message
git tag -a v1.0.0 -m "Version 1.0.0 release"

# Push tags
git push origin v1.0.0
git push origin --tags  # All tags

# List tags
git tag -l
```

### Undo and Reset

```bash
# Soft reset (keep changes)
git reset --soft HEAD~1

# Mixed reset (keep changes staged)
git reset --mixed HEAD~1

# Hard reset (remove all changes)
git reset --hard HEAD~1

# Discard changes
git checkout -- index.html

# Discard all local changes
git reset --hard
```

## 📦 GitHub Operations

### Create Pull Request

```bash
# Push your branch first
git push origin feature/YourFeature

# Go to GitHub and create PR
# Or use CLI:
gh pr create --title "PR Title" --body "Description"
```

### View PRs

```bash
# List your PRs
gh pr list

# View specific PR
gh pr view 1
```

## 🔍 File Search and Discovery

### View File Structure

```bash
# List all files
ls -la

# Directory tree
tree -L 2

# Find all files
find . -type f
```

### Search Content

```bash
# Search in all files
grep -r "searchTerm" .

# Search specific file types
grep -r "searchTerm" --include="*.js"

# Case-insensitive
grep -ri "searchTerm" .

# Show line numbers
grep -rn "searchTerm" .
```

## 🗑️ File Management

### Create Files

```bash
# Create empty file
touch newfile.js

# Create with content
echo "// comment" > newfile.js
```

### Edit Files

```bash
# nano editor
nano index.html

# vim editor
vim index.html

# Open in VS Code
code .
```

### Delete Files

```bash
# Delete file
rm index.html

# Confirm before delete
rm -i index.html

# Delete directory
rm -r dirname
```

## 🚀 Deployment Commands

### GitHub Pages (Automatic)

```bash
# Just push to main
git push origin main

# GitHub Pages updates automatically (2-5 minutes)
# https://shanto008sb.github.io/Hacker_Kal_AI/
```

## 💡 Quick Tips

```bash
# Everything in one line
git add . && git commit -m "fix" && git push origin main

# Go back to previous commit
git checkout <commit-hash>

# Stash and apply
git stash
git stash pop

# Current branch name
git rev-parse --abbrev-ref HEAD
```

---

**Last Updated**: June 28, 2026  
For more help: `git help [command]`