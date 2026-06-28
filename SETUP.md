# 🛠️ Setup Guide

Complete setup and installation instructions for Hacker_Kal_AI.

## ✅ Prerequisites

- Git installed (Download: https://git-scm.com)
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection
- Text editor (VS Code, Sublime, Atom, etc.)

---

## 1️⃣ Step One: GitHub Setup

### 1.1 Create GitHub Account

```bash
# Go to https://github.com and sign up
```

### 1.2 Configure Git

```bash
# Set your name and email
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# Verify
git config --list
```

### 1.3 Setup SSH Key (Optional but Recommended)

```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "your@email.com"

# Press Enter for all defaults
# Set passphrase if desired

# View public key
cat ~/.ssh/id_ed25519.pub

# Go to GitHub → Settings → SSH Keys → Add New
# Copy the key above
```

---

## 2️⃣ Step Two: Repository Setup

### 2.1 Clone Repository

```bash
# HTTPS (easy)
git clone https://github.com/Shanto008SB/Hacker_Kal_AI.git

# SSH (faster after SSH setup)
git clone git@github.com:Shanto008SB/Hacker_Kal_AI.git

# Go to directory
cd Hacker_Kal_AI
```

### 2.2 Verify Files

```bash
# List files
ls -la

# Should show:
# README.md
# SECURITY.md
# index.html
# styles.css
# script.js
# .github/
```

### 2.3 Verify Remote

```bash
# Check remote connection
git remote -v

# Should show:
# origin  https://github.com/Shanto008SB/Hacker_Kal_AI.git (fetch)
# origin  https://github.com/Shanto008SB/Hacker_Kal_AI.git (push)
```

---

## 3️⃣ Step Three: Local Server Setup

### Option A: Live Server (VS Code) - Best

```bash
# 1. Download VS Code: https://code.visualstudio.com
# 2. Install and open
# 3. Open Extensions (Ctrl+Shift+X)
# 4. Search "Live Server" and install
# 5. Right-click index.html → "Open with Live Server"
# 6. Opens at http://localhost:5500
```

### Option B: Python

```bash
# Check if Python installed
python --version

# Python 3.x
python -m http.server 8000

# Browser: http://localhost:8000
```

### Option C: Node.js

```bash
# Download: https://nodejs.org
# Check: node --version

# Install http-server
npm install -g http-server

# Run
http-server

# Browser: http://localhost:8080
```

### Option D: PHP

```bash
# Download: https://www.php.net/downloads.php
# Check: php --version

# Run
php -S localhost:8000

# Browser: http://localhost:8000
```

---

## 4️⃣ Step Four: Editor Setup

### VS Code Setup (Recommended)

```bash
# 1. Download: https://code.visualstudio.com
# 2. Install and open

# 3. Install extensions:
#    - Live Server
#    - HTML Preview
#    - CSS Peek
#    - JavaScript (ES6) Code Snippets
#    - Prettier

# 4. Open folder:
#    File → Open Folder → Select Hacker_Kal_AI

# 5. Start editing
```

### Other Editors

```bash
# Sublime Text: https://www.sublimetext.com
# Atom: https://atom.io
# Nano (command line): nano index.html
# Vim (advanced): vim index.html
```

---

## 5️⃣ Step Five: Test and Verify

### 5.1 Browser Testing

```bash
# Open in all browsers and test:
# Chrome, Firefox, Safari, Edge
# Check: http://localhost:8000
```

### 5.2 Edit File Test

```bash
# Make a change to index.html
# Server auto-reloads
# Verify change appears
```

### 5.3 Check Console

```bash
# Open Developer Tools (F12)
# Go to Console tab
# Check for any errors
```

---

## 6️⃣ Step Six: First Commit

### 6.1 Create Your Fork (If Contributing)

```bash
# Go to GitHub
# https://github.com/Shanto008SB/Hacker_Kal_AI
# Click "Fork" button
```

### 6.2 Make Changes and Commit

```bash
# Create or edit a test file
echo "// test" > test.js

# Check status
git status

# Stage
git add .

# Commit
git commit -m "test: Add test file"

# Push
git push origin main

# Check GitHub - changes are there!
```

---

## 7️⃣ Step Seven: Development Workflow

### Standard Workflow

```bash
# 1. Get latest updates
git pull origin main

# 2. Create branch
git checkout -b feature/MyNewFeature

# 3. Work (edit files)

# 4. Check status
git status

# 5. Stage
git add .

# 6. Commit
git commit -m "feat: Add new feature"

# 7. Push
git push origin feature/MyNewFeature

# 8. Create Pull Request on GitHub
```

---

## 🚨 Common Issues and Solutions

### Issue 1: "Permission denied (publickey)"

```bash
# Solution: Setup SSH key
ssh-keygen -t ed25519 -C "your@email.com"
# Add key to GitHub Settings
```

### Issue 2: "fatal: not a git repository"

```bash
# Solution: Make sure you're in correct directory
pwd  # Show current path
cd Hacker_Kal_AI  # Go to correct folder
```

### Issue 3: Port already in use

```bash
# Solution: Use different port
python -m http.server 9000  # Instead of 8000

# Or stop the server:
# Press Ctrl+C in terminal
```

### Issue 4: File merge conflict

```bash
# Solution: Resolve conflict
git status  # See conflicted files

# Manually fix the file
nano filename

# Then
git add filename
git commit -m "fix: Resolve merge conflict"
```

---

## 📚 Next Steps

1. **Read README.md**: Understand the project
2. **Read COMMANDS.md**: All command reference
3. **Read CONTRIBUTING.md**: How to contribute
4. **Explore Code**: Check index.html, styles.css, script.js

---

**Good luck! Happy coding! 🚀**