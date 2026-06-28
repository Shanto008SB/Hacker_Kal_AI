# 🛠️ সমস্ত কমান্ড রেফারেন্স

Hacker_Kal_AI এর জন্য সমস্ত ব্যবহারকারী কমান্ড এবং ডেভেলপার কমান্ড।

## 📥 ক্লোনিং এবং সেটআপ

### রিপোজিটরি ক্লোন করুন

```bash
# HTTPS এর মাধ্যমে
git clone https://github.com/Shanto008SB/Hacker_Kal_AI.git

# SSH এর মাধ্যমে
git clone git@github.com:Shanto008SB/Hacker_Kal_AI.git

# GitHub CLI এর মাধ্যমে
gh repo clone Shanto008SB/Hacker_Kal_AI
```

### ডিরেক্টরিতে প্রবেশ করুন

```bash
cd Hacker_Kal_AI
```

## 🚀 লোকাল সার্ভার চালান

### অপশন 1: Live Server (VS Code) - সুপারিশকৃত

```bash
# VS Code এ:
# 1. Live Server এক্সটেনশন ইনস্টল করুন
# 2. index.html এ রাইট-ক্লিক → "Open with Live Server"
```

### অপশন 2: Python হোস্ট করুন

```bash
# Python 3.x
python -m http.server 8000

# Python 2.x
python -m SimpleHTTPServer 8000

# তারপর ব্রাউজারে খুলুন: http://localhost:8000
```

### অপশন 3: Node.js হোস্ট করুন

```bash
# http-server ইনস্টল করুন (প্রথমবার)
npm install -g http-server

# চালান
http-server

# বা port নির্দিষ্ট করুন
http-server -p 3000
```

### অপশন 4: PHP হোস্ট করুন

```bash
# PHP 5.4+
php -S localhost:8000

# তারপর ব্রাউজারে খুলুন: http://localhost:8000
```

## 🔧 গিট কমান্ড

### ব্রাঞ্চ পরিচালনা

```bash
# নতুন ব্রাঞ্চ তৈরি করুন
git checkout -b feature/NewFeature

# শাখা তালিকা দেখুন
git branch -a

# শাখা মুছুন
git branch -d feature/NewFeature
git branch -D feature/NewFeature  # বাধ্যতামূলক মুছুন
```

### পরিবর্তন কমিট করুন

```bash
# সব ফাইল যোগ করুন
git add .

# নির্দিষ্ট ফাইল যোগ করুন
git add index.html

# পরিবর্তন দেখুন
git status

# কমিট করুন
git commit -m "feat: নতুন ফিচার যোগ করুন"

# বিস্তারিত বার্তা সহ কমিট করুন
git commit -m "feat: নতুন AI ফিচার
- AI চ্যাট ইন্টারফেস যোগ করা হয়েছে
- নতুন UI উপাদান যোগ করা হয়েছে"
```

### পুশ এবং পুল

```bash
# GitHub এ পুশ করুন
git push origin main

# শাখা পুশ করুন
git push origin feature/NewFeature

# GitHub থেকে পুল করুন
git pull origin main

# Force Push (সাবধানে!)
git push origin main --force
```

### লজ এবং ইতিহাস

```bash
# কমিট ইতিহাস দেখুন
git log

# সুন্দর লজ ফরম্যাট
git log --oneline --graph --all

# নির্দিষ্ট ফাইল পরিবর্তন দেখুন
git log -p index.html

# সম্প্রতি পরিবর্তন দেখুন
git diff

# নির্দিষ্ট ফাইল পার্থক্য দেখুন
git diff index.html
```

### সংস্করণ ট্যাগ

```bash
# নতুন ট্যাগ তৈরি করুন
git tag v1.0.0

# মন্তব্য সহ ট্যাগ
git tag -a v1.0.0 -m "Version 1.0.0 রিলিজ"

# ট্যাগ পুশ করুন
git push origin v1.0.0
git push origin --tags  # সব ট্যাগ পুশ করুন

# ট্যাগ তালিকা দেখুন
git tag -l
```

### বাতিল এবং রিসেট

```bash
# সর্বশেষ কমিট বাতিল করুন (রাখা পরিবর্তন)
git reset --soft HEAD~1

# সর্বশেষ কমিট বাতিল করুন (স্টেজিং রাখা)
git reset --mixed HEAD~1

# সর্বশেষ কমিট সম্পূর্ণ বাতিল করুন
git reset --hard HEAD~1

# পরিবর্তন বাতিল করুন
git checkout -- index.html

# সব স্থানীয় পরিবর্তন বাতিল করুন
git reset --hard
```

## 📦 GitHub অপারেশন

### Pull Request তৈরি করুন

```bash
# ব্রাউজারে GitHub যান
# 1. আপনার ফর্ক খুলুন
# 2. "New Pull Request" ক্লিক করুন
# 3. টাইটেল এবং বর্ণনা যোগ করুন
# 4. "Create Pull Request" ক্লিক করুন
```

### CLI দিয়ে PR তৈরি করুন

```bash
# GitHub CLI সহ
gh pr create --title "নতুন ফিচার" --body "বর্ণনা"

# আপনার PR দেখুন
gh pr list

# নির্দিষ্ট PR দেখুন
gh pr view 1
```

## 🔍 অনুসন্ধান এবং পরিদর্শন

### ফাইল গঠন দেখুন

```bash
# সব ফাইল দেখুন
ls -la

# ডিরেক্টরি গঠন দেখুন (ট্রি কমান্ড)
tree -L 2

# লুকানো ফাইল সহ
find . -type f
```

### কন্টেন্ট অনুসন্ধান করুন

```bash
# সমস্ত ফাইলে খুঁজুন
grep -r "searchTerm" .

# নির্দিষ্ট ফাইল প্রকারে খুঁজুন
grep -r "searchTerm" --include="*.js"

# কেস-সংবেদনশীল নয়
grep -ri "searchTerm" .

# লাইন নম্বর দেখান
grep -rn "searchTerm" .
```

## 🗑️ ফাইল পরিচালনা

### ফাইল তৈরি করুন

```bash
# নতুন ফাইল তৃতীয় করুন
touch newfile.js

# বিষয়বস্তু সহ তৃতীয় করুন
echo "// নতুন ফাইল" > newfile.js
```

### ফাইল সম্পাদনা করুন

```bash
# nano সম্পাদক
nano index.html

# vim সম্পাদক
vim index.html

# VS Code খুলুন
code .
```

### ফাইল মুছুন

```bash
# একটি ফাইল মুছুন
rm index.html

# একটি ফাইল মুছুন (নিশ্চিত)
rm -i index.html

# ডিরেক্টরি মুছুন
rm -r dirname
```

## 🚀 ডেপ্লয়মেন্ট কমান্ড

### GitHub Pages (স্বয়ংক্রিয়)

```bash
# শুধুমাত্র GitHub এ পুশ করুন
git push origin main

# GitHub Pages স্বয়ংক্রিয়ভাবে আপডেট হবে (2-5 মিনিটে)
# https://shanto008sb.github.io/Hacker_Kal_AI/
```

### কাস্টম ডোমেইনে

```bash
# CNAME ফাইল তৃতীয় করুন
echo "yourdomain.com" > CNAME

# কমিট এবং পুশ করুন
git add CNAME
git commit -m "feat: কাস্টম ডোমেইন যোগ করুন"
git push origin main
```

## 📊 অন্যান্য উপযোগী কমান্ড

### রিমোট রিপোজিটরি পরিচালনা

```bash
# রিমোট দেখুন
git remote -v

# নতুন রিমোট যোগ করুন
git remote add upstream https://github.com/ORIGINAL_OWNER/REPO.git

# রিমোট সিঙ্ক করুন
git fetch upstream
git merge upstream/main
```

### ফাইল পার্মিশন

```bash
# বাস্তবায়ন যোগ্য করুন
chmod +x script.js

# পাঠযোগ্য করুন
chmod 644 index.html
```

### সার্ভার পরিচালনা বন্ধ করুন

```bash
# Ctrl+C ব্যবহার করুন (সব সিস্টেমে)
# টার্মিনালে Ctrl+C প্রেস করুন

# পোর্ট খুঁজুন এবং বন্ধ করুন
lsof -i :8000  # ফাইন্ড প্রসেস
kill -9 PID    # প্রসেস বন্ধ করুন
```

## 💡 দ্রুত টিপস

```bash
# সব এক লাইনে
git add . && git commit -m "ফিক্স" && git push origin main

# একটি পূর্ববর্তী সংস্করণে ফিরে যান
git checkout <commit-hash>

# স্টেশ এবং পরে প্রয়োগ করুন
git stash
git stash pop

# বর্তমান শাখার নাম দেখুন
git rev-parse --abbrev-ref HEAD
```

---

**শেষ আপডেট**: 28 জুন, 2026  
আরও সাহায্যের জন্য: `git help [command]`