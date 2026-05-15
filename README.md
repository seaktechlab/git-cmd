````markdown
# ACLEDA Mobile iOS

iOS mobile application project for ACLEDA.

---

# Git Global Setup

Before cloning project, configure your Git account.

## Set Git Username

```bash
git config --global user.name "Your Name"
```

Example:

```bash
git config --global user.name "Kimseak Phorn"
```

---

## Set Git Email

```bash
git config --global user.email "your_email@example.com"
```

Example:

```bash
git config --global user.email "kimseak@example.com"
```

---

## Verify Git Configuration

```bash
git config --global --list
```

---

# Requirements

- macOS
- Xcode
- CocoaPods
- Git

---

# Clone Project

Open Terminal and run:

```bash
cd /your-project

git clone http://10.11.20.251/kimseak/acleda-mobile-ios.git
```

Example:

```bash
cd Desktop

git clone http://10.11.20.251/kimseak/acleda-mobile-ios.git
```

After clone complete:

```bash
cd acleda-mobile-ios
```

---

# Setup Project

## 1. Install CocoaPods

```bash
pod install
```

If pod command not found:

```bash
sudo gem install cocoapods
```

---

## 2. Open Project

Open workspace file:

```bash
open YourProject.xcworkspace
```

Important:

- Always open `.xcworkspace`
- Do not open `.xcodeproj` when using CocoaPods

---

## 3. Resolve Swift Package Manager (SPM)

In Xcode:

- File
- Packages
- Resolve Package Versions

Or wait for Xcode to automatically download packages.

---

# Git Workflow

## Check Current Branch

```bash
git branch
```

---

## Pull Latest Develop

```bash
git checkout develop
git pull origin develop
```

---

## Create New Branch

Recommended branch naming:

```bash
git checkout -b feature/login-improvement
```

Examples:

```bash
git checkout -b feature/home-ui
git checkout -b bugfix/payment-crash
git checkout -b hotfix/api-timeout
```

---

# Daily Development Flow

## Start Working

```bash
git checkout develop
git pull origin develop

git checkout your-branch
git merge develop
```

---

# Commit Code

## Check Changed Files

```bash
git status
```

---

## Add Files

Add all files:

```bash
git add .
```

Or specific file:

```bash
git add Sources/HomeViewController.swift
```

---

## Commit Changes

Recommended commit format:

```bash
git commit -m "feat: improve login validation"
```

Examples:

```bash
git commit -m "fix: resolve startup crash"
git commit -m "refactor: clean payment logic"
git commit -m "chore: update dependencies"
```

---

# Push Code

First push:

```bash
git push -u origin feature/login-improvement
```

Next pushes:

```bash
git push
```

---

# Merge Request (MR)

1. Open GitLab
2. Go to Merge Requests
3. Click New Merge Request
4. Select:
   - Source branch = your branch
   - Target branch = develop
5. Add:
   - Title
   - Description
6. Create Merge Request

---

# Best Practices

- Never commit directly to `main` or `master`
- Use feature branches
- Pull latest `develop` before coding
- Review changed files before push
- Use meaningful commit messages
- Keep branch focused on one task

---

# Recommended Branch Structure

```text
develop
 ├── feature/login
 ├── feature/home-ui
 ├── bugfix/payment
 └── hotfix/api
```

---

# Useful Git Commands

## Check Status

```bash
git status
```

## Check Branches

```bash
git branch
```

## View Commit History

```bash
git log --oneline
```

## Pull Latest Code

```bash
git pull
```

## Push Code

```bash
git push
```

---

# Troubleshooting

## Pod Install Failed

Try:

```bash
pod repo update
pod install
```

---

## Clean Build

```bash
Shift + Command + K
```

---

## Remove Derived Data

```bash
rm -rf ~/Library/Developer/Xcode/DerivedData
```

---

# Author

ACLEDA Mobile iOS Team
````
