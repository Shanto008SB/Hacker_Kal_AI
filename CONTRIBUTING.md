# অবদান রাখার গাইড

ধন্যবাদ Hacker_Kal_AI প্রজেক্টে অবদান রাখার আগ্রহের জন্য! 🎉

## কোড অবদান প্রক্রিয়া

### 1. রিপোজিটরি ফর্ক করুন

```bash
# GitHub এ যান এবং "Fork" বোতাম ক্লিক করুন
# অথবা CLI তে:
gh repo fork Shanto008SB/Hacker_Kal_AI --clone
```

### 2. ক্লোন করুন এবং ব্রাঞ্চ তৈরি করুন

```bash
git clone https://github.com/YOUR_USERNAME/Hacker_Kal_AI.git
cd Hacker_Kal_AI

# নতুন ব্রাঞ্চ তৈরি করুন
git checkout -b feature/YourFeatureName
```

### 3. পরিবর্তন করুন

```bash
# ফাইল সম্পাদনা করুন
# স্থানীয় পরীক্ষা করুন

# পরিবর্তন পর্যায়ে রাখুন
git add .

# কমিট করুন
git commit -m "সংক্ষিপ্ত এবং বর্ণনামূলক বার্তা"
```

### 4. Push করুন এবং PR তৈরি করুন

```bash
git push origin feature/YourFeatureName
```

GitHub এ যান এবং Pull Request তৈরি করুন।

## প্রতিবেদন করার জন্য

### বাগ রিপোর্ট

1. [Issues](https://github.com/Shanto008SB/Hacker_Kal_AI/issues) যান
2. "New Issue" ক্লিক করুন
3. টেমপ্লেট পূরণ করুন:

```markdown
## বাগের বর্ণনা
সংক্ষিপ্ত বিবরণ

## পুনরুৎপাদনের ধাপ
1. যান '...'
2. ক্লিক করুন '....'
3. দেখুন ত্রুটি '....'

## প্রত্যাশিত আচরণ
কি ঘটা উচিত ছিল

## প্রকৃত আচরণ
কি আসলে ঘটেছে

## ব্রাউজার/OS তথ্য
- ব্রাউজার: Chrome 120
- OS: Windows 11
```

### ফিচার অনুরোধ

```markdown
## ফিচারের বর্ণনা
এটি কি করবে

## সমস্যা সমাধান করে
এটি কোন সমস্যার সমাধান করে

## প্রস্তাবিত সমাধান
আপনার ধারণা
```

## কোডিং মান

### HTML/CSS/JavaScript স্টাইল

```javascript
// ভাল: স্পষ্ট নাম এবং মন্তব্য
function analyzeTarget(targetUrl) {
  // URL বৈধতা
  if (!isValidUrl(targetUrl)) {
    return null;
  }
  // বিশ্লেষণ লজিক
  return performAnalysis(targetUrl);
}
```

### মন্তব্য যোগ করুন

```html
<!-- প্রধান ইউজার ইনপুট সেকশন -->
<div id="target-input-section" class="mb-8">
  <!-- টার্গেট ইনপুট ফিল্ড -->
  <input type="text" id="target-input" placeholder="Enter target">
</div>
```

## কমিট বার্তার নিয়ম

```bash
# ফর্ম্যাট: [TYPE] সংক্ষিপ্ত বর্ণনা
# উদাহরণ:

git commit -m "feat: নতুন AI চ্যাট ফিচার যোগ করুন"
git commit -m "fix: কপি বোতাম বাগ সংশোধন"
git commit -m "docs: README আপডেট"
git commit -m "style: CSS ফরম্যাটিং উন্নত করুন"
git commit -m "refactor: script.js পুনর্সংগঠন"
git commit -m "test: নতুন ওয়ার্কফ্লো পরীক্ষা"
```

## টাইপ

- `feat`: নতুন ফিচার
- `fix`: বাগ ফিক্স
- `docs`: ডকুমেন্টেশন পরিবর্তন
- `style`: কোডিং স্টাইল (বিন্যাস, মিসিং semicolons, ইত্যাদি)
- `refactor`: কোড পুনর্লিখন (কার্যকারিতা পরিবর্তন ছাড়া)
- `perf`: পারফরম্যান্স উন্নতি
- `test`: পরীক্ষা যোগ করুন

## পরীক্ষা করার কথা

1. **ব্রাউজার সামঞ্জস্য**: Chrome, Firefox, Safari, Edge
2. **প্রতিক্রিয়াশীলতা**: ডেস্কটপ এবং মোবাইল
3. **কর্মক্ষমতা**: পেজ লোড সময়
4. **অ্যাক্সেসযোগ্যতা**: কীবোর্ড নেভিগেশন

## শাখার নামকরণ সম্মেলন

```bash
feature/description      # নতুন ফিচার
bugfix/description       # বাগ ফিক্স
docs/description         # ডকুমেন্টেশন
refactor/description     # কোড পুনর্গঠন
```

## PR চেকলিস্ট

- [ ] কোড স্টাইল অনুসরণ করেছি
- [ ] স্বয়ংক্রিয় পরীক্ষা পাস করেছি
- [ ] নতুন এবং বিদ্যমান উভয় ফিচার পরীক্ষা করেছি
- [ ] নথিপত্র আপডেট করেছি
- [ ] কোন অপ্রয়োজনীয় মন্তব্য সরিয়েছি

## যোগাযোগ

- প্রশ্ন থাকলে Issues ব্যবহার করুন
- Discussions এ আলোচনা করতে পারেন

ধন্যবাদ! 🙏