# 🛠️ সেটআপ গাইড

Hacker_Kal_AI এর জন্য সম্পূর্ণ সেটআপ এবং ইনস্টলেশন নির্দেশাবলী।

## ✅ পূর্বশর্ত

- Git ইনস্টল করা (ডাউনলোড: https://git-scm.com)
- একটি আধুনিক ওয়েব ব্রাউজার (Chrome, Firefox, Safari, Edge)
- ইন্টারনেট সংযোগ
- একটি টেক্সট এডিটর (VS Code, Sublime, Atom ইত্যাদি)

---

## 1️⃣ প্রথম ধাপ: GitHub সেটআপ

### 1.1 GitHub অ্যাকাউন্ট তৈরি করুন

```bash
# https://github.com এ যান এবং সাইন আপ করুন
```

### 1.2 Git কনফিগার করুন

```bash
# আপনার নাম এবং ইমেইল সেট করুন
git config --global user.name "আপনার নাম"
git config --global user.email "আপনার@email.com"

# যাচাই করুন
git config --list
```

### 1.3 SSH কী সেটআপ করুন (ঐচ্ছিক কিন্তু সুপারিশকৃত)

```bash
# SSH কী তৈরি করুন
ssh-keygen -t ed25519 -C "আপনার@email.com"

# সব ডিফল্ট অপশন চাপুন (Enter)
# পাসফ্রেজ সেট করুন বা এন্টার প্রেস করুন

# পাবলিক কী দেখুন
cat ~/.ssh/id_ed25519.pub

# GitHub এ যান → Settings → SSH Keys → Add New
# উপরের কী কপি-পেস্ট করুন
```

---

## 2️⃣ দ্বিতীয় ধাপ: রিপোজিটরি সেটআপ

### 2.1 রিপোজিটরি ক্লোন করুন

```bash
# HTTPS ব্যবহার করে (সহজ)
git clone https://github.com/Shanto008SB/Hacker_Kal_AI.git

# অথবা SSH ব্যবহার করে (দ্রুত)
git clone git@github.com:Shanto008SB/Hacker_Kal_AI.git

# ডিরেক্টরিতে যান
cd Hacker_Kal_AI
```

### 2.2 ফাইল গঠন পরীক্ষা করুন

```bash
# ফাইল তালিকা দেখুন
ls -la

# আউটপুট:
# README.md
# SECURITY.md
# index.html
# styles.css
# script.js
# .github/
# .gitignore (যদি থাকে)
```

### 2.3 রিমোট যাচাই করুন

```bash
# রিমোট সংযোগ দেখুন
git remote -v

# আউটপুট:
# origin  https://github.com/Shanto008SB/Hacker_Kal_AI.git (fetch)
# origin  https://github.com/Shanto008SB/Hacker_Kal_AI.git (push)
```

---

## 3️⃣ তৃতীয় ধাপ: স্থানীয় সার্ভার সেটআপ

### অপশন A: Live Server (VS Code) - সর্বোত্তম

```bash
# 1. VS Code ডাউনলোড করুন (https://code.visualstudio.com)
# 2. এক্সটেনশন খুলুন (Ctrl+Shift+X)
# 3. "Live Server" খুঁজুন → Ritwick Dey দ্বারা ইনস্টল করুন
# 4. index.html এ রাইট-ক্লিক → "Open with Live Server"
# 5. http://localhost:5500 এ খোলা হবে
```

### অপশন B: Python হোস্ট করুন

```bash
# চেক করুন Python ইনস্টল করা আছে
python --version

# Python 3.x এর সাথে সার্ভার চালান
python -m http.server 8000

# ব্রাউজারে খুলুন: http://localhost:8000
```

### অপশন C: Node.js হোস্ট করুন

```bash
# Node.js ইনস্টল করুন (https://nodejs.org)
# চেক করুন
node --version

# http-server ইনস্টল করুন
npm install -g http-server

# চালান
http-server

# ব্রাউজারে খুলুন: http://localhost:8080
```

### অপশন D: PHP হোস্ট করুন

```bash
# PHP ইনস্টল করুন (https://www.php.net/downloads.php)
# চেক করুন
php --version

# চালান
php -S localhost:8000

# ব্রাউজারে খুলুন: http://localhost:8000
```

---

## 4️⃣ চতুর্থ ধাপ: সম্পাদক সেটআপ

### VS Code সেটআপ (সুপারিশকৃত)

```bash
# 1. VS Code ডাউনলোড করুন: https://code.visualstudio.com
# 2. ইনস্টল করুন এবং খুলুন

# 3. প্রয়োজনীয় এক্সটেনশন ইনস্টল করুন:
#    - Live Server (সার্ভার চালানোর জন্য)
#    - HTML Preview
#    - CSS Peek
#    - JavaScript (ES6) Code Snippets
#    - Prettier (কোড ফরম্যাটার)

# 4. ফোল্ডার খুলুন:
#    File → Open Folder → Hacker_Kal_AI নির্বাচন করুন

# 5. সম্পাদনা শুরু করুন
```

### অন্যান্য সম্পাদক

```bash
# Sublime Text
# ডাউনলোড: https://www.sublimetext.com
# প্লাগইন: Package Control → HTML/CSS/JS Prettier

# Atom
# ডাউনলোড: https://atom.io
# প্যাকেজ: live-server, prettier-atom

# Nano (কমান্ড লাইন)
nano index.html

# Vim (উন্নত)
vim index.html
```

---

## 5️⃣ পঞ্চম ধাপ: পরীক্ষা এবং যাচাই করা

### 5.1 ব্রাউজার পরীক্ষা করুন

```bash
# সব ব্রাউজারে খুলুন এবং পরীক্ষা করুন:

# Chrome: Google Chrome খুলুন → http://localhost:8000
# Firefox: Mozilla Firefox খুলুন → http://localhost:8000
# Safari: Safari খুলুন → http://localhost:8000
# Edge: Microsoft Edge খুলুন → http://localhost:8000
```

### 5.2 ফাইল সম্পাদনা পরীক্ষা করুন

```bash
# index.html এ একটি পরিবর্তন করুন
# সার্ভার স্বয়ংক্রিয়ভাবে রিলোড হবে

# উদাহরণ: লাইন 27 অনুসরণ করুন
# <h1> ট্যাগে কিছু যোগ করুন এবং দেখুন পরিবর্তন হয়েছে
```

### 5.3 কনসোল ত্রুটি পরীক্ষা করুন

```bash
# ব্রাউজার ডেভেলপার টুলস খুলুন (F12 বা Ctrl+Shift+I)
# Console ট্যাব দেখুন
# কোন ত্রুটি দেখা যায় না? ভালো!
```

---

## 6️⃣ ষষ্ঠ ধাপ: প্রথম কমিট এবং পুশ

### 6.1 আপনার ফর্ক তৈরি করুন (যদি আপনি অবদান রাখতে চান)

```bash
# GitHub এ যান
# https://github.com/Shanto008SB/Hacker_Kal_AI

# "Fork" বোতাম ক্লিক করুন
# আপনার অ্যাকাউন্টে কপি তৈরি হবে
```

### 6.2 পরিবর্তন করুন এবং কমিট করুন

```bash
# একটি নতুন ফাইল তৈরি করুন বা সম্পাদনা করুন
echo "// টেস্ট ফাইল" > test.js

# পরিবর্তন দেখুন
git status

# স্টেজ করুন
git add .

# কমিট করুন
git commit -m "test: টেস্ট ফাইল যোগ করুন"

# পুশ করুন
git push origin main

# GitHub এ চেক করুন - পরিবর্তন দেখা যাবে!
```

---

## 7️⃣ সপ্তম ধাপ: উন্নয়ন ওয়ার্কফ্লো

### সাধারণ কর্মপ্রবাহ

```bash
# ১. সর্বশেষ আপডেট পান
git pull origin main

# ২. নতুন ব্রাঞ্চ তৈরি করুন
git checkout -b feature/MyNewFeature

# ৩. কাজ করুন (ফাইল সম্পাদনা করুন)

# ৪. পরিবর্তন দেখুন
git status

# ৫. স্টেজ করুন
git add .

# ৬. কমিট করুন
git commit -m "feat: নতুন ফিচার যোগ করুন"

# ৭. পুশ করুন
git push origin feature/MyNewFeature

# ৮. GitHub এ Pull Request তৈরি করুন
```

---

## 🚨 সাধারণ সমস্যা এবং সমাধান

### সমস্যা 1: "Permission denied (publickey)"

```bash
# সমাধান: SSH কী সেটআপ করুন
ssh-keygen -t ed25519 -C "আপনার@email.com"
# GitHub Settings → SSH Keys → কী যোগ করুন
```

### সমস্যা 2: "fatal: not a git repository"

```bash
# সমাধান: সঠিক ডিরেক্টরিতে আছেন তা নিশ্চিত করুন
pwd  # বর্তমান পথ দেখুন
cd Hacker_Kal_AI  # সঠিক ফোল্ডারে যান
```

### সমস্যা 3: পোর্ট ইতিমধ্যে ব্যবহৃত

```bash
# সমাধান: অন্য পোর্ট ব্যবহার করুন
python -m http.server 9000  # 8000 এর বদলে 9000

# অথবা প্রসেস বন্ধ করুন
# Ctrl+C টার্মিনালে প্রেস করুন
```

### সমস্যা 4: ফাইল মার্জ সংঘর্ষ

```bash
# সমাধান: সংঘর্ষ সমাধান করুন
git status  # সংঘর্ষযুক্ত ফাইল দেখুন

# ম্যানুয়ালি সমাধান করুন
nano filename

# তারপর
git add filename
git commit -m "fix: মার্জ সংঘর্ষ সমাধান করুন"
```

---

## 📚 পরবর্তী পদক্ষেপ

1. **README.md পড়ুন**: প্রজেক্ট বুঝতে
2. **COMMANDS.md পড়ুন**: সমস্ত কমান্ড রেফারে��্স
3. **CONTRIBUTING.md পড়ুন**: অবদান কিভাবে রাখবেন
4. **কোড অন্বেষণ করুন**: index.html, styles.css, script.js দেখুন

---

## ✨ দ্রুত রেফারেন্স

```bash
# সেটআপ (এক বার)
git clone https://github.com/Shanto008SB/Hacker_Kal_AI.git
cd Hacker_Kal_AI
python -m http.server 8000

# প্রতিদিনের কমান্ড
git pull origin main          # আপডেট পান
nano index.html               # সম্পাদনা করুন
git add . && git commit -m "msg" && git push  # পুশ করুন
```

---

## 🆘 সাহায্যের জন্য

- **প্রশ্ন থাকলে**: [Issues](https://github.com/Shanto008SB/Hacker_Kal_AI/issues) খুলুন
- **আরও তথ্য**: [GitHub ডকুমেন্টেশন](https://docs.github.com)
- **Git টিউটোরিয়াল**: [Pro Git Book](https://git-scm.com/book)

---

**শুভকামনা! হ্যাপি কোডিং! 🚀**