# Contributing Guide

Thank you for your interest in contributing to Hacker_Kal_AI! 🎉

## Code Contribution Process

### 1. Fork the Repository

```bash
# Go to GitHub and click "Fork" button
# Or use CLI:
gh repo fork Shanto008SB/Hacker_Kal_AI --clone
```

### 2. Clone and Create Branch

```bash
git clone https://github.com/YOUR_USERNAME/Hacker_Kal_AI.git
cd Hacker_Kal_AI

# Create new branch
git checkout -b feature/YourFeatureName
```

### 3. Make Changes

```bash
# Edit files
# Test locally

# Stage changes
git add .

# Commit
git commit -m "Clear descriptive message"
```

### 4. Push and Create PR

```bash
git push origin feature/YourFeatureName
```

Go to GitHub and create a Pull Request.

## Reporting Issues

### Bug Report

1. Visit [Issues](https://github.com/Shanto008SB/Hacker_Kal_AI/issues)
2. Click "New Issue"
3. Fill the template:

```markdown
## Bug Description
Clear description

## Steps to Reproduce
1. Go to '...'
2. Click '...'
3. See error '...'

## Expected Behavior
What should happen

## Actual Behavior
What actually happened

## Browser/OS Info
- Browser: Chrome 120
- OS: Windows 11
```

### Feature Request

```markdown
## Feature Description
What it should do

## Problem it solves
The issue it addresses

## Proposed Solution
Your idea
```

## Coding Standards

### HTML/CSS/JavaScript Style

```javascript
// Good: Clear names and comments
function analyzeTarget(targetUrl) {
  // Validate URL
  if (!isValidUrl(targetUrl)) {
    return null;
  }
  // Analysis logic
  return performAnalysis(targetUrl);
}
```

### Add Comments

```html
<!-- Main user input section -->
<div id="target-input-section" class="mb-8">
  <!-- Target input field -->
  <input type="text" id="target-input" placeholder="Enter target">
</div>
```

## Commit Message Format

```bash
# Format: [TYPE] brief description
# Examples:

git commit -m "feat: Add new AI chat feature"
git commit -m "fix: Resolve copy button bug"
git commit -m "docs: Update README"
git commit -m "style: Improve CSS formatting"
git commit -m "refactor: Reorganize script.js"
git commit -m "test: Add new workflow tests"
```

## Types

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style (formatting, missing semicolons)
- `refactor`: Code refactoring (without functionality changes)
- `perf`: Performance improvement
- `test`: Add tests

## Testing Checklist

1. **Browser Compatibility**: Chrome, Firefox, Safari, Edge
2. **Responsiveness**: Desktop and mobile
3. **Performance**: Page load time
4. **Accessibility**: Keyboard navigation

## Branch Naming Convention

```bash
feature/description      # New feature
bugfix/description       # Bug fix
docs/description         # Documentation
refactor/description     # Code refactoring
```

## PR Checklist

- [ ] Followed code style
- [ ] Tested on all browsers
- [ ] Updated documentation
- [ ] No unnecessary comments

## Communication

- Use Issues for questions
- Discussions for ideas

Thank you! 🙏