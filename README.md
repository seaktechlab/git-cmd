# ACLEDA Mobile iOS

iOS mobile application project for ACLEDA.

---

## Requirements

Before setup, ensure the following are installed:

- macOS
- Xcode
- Git
- CocoaPods

---

# Git Global Setup

Configure Git before cloning the project.

## Set Username

```bash
git config --global user.name "Your Name"
```

Example:

```bash
git config --global user.name "Kimseak Phorn"
```

---

## Set Email

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

# Clone Project

```bash
cd /your-project

git clone http://localserverip/kimseak/repo-name.git
```

Example:

```bash
cd Desktop

git clone http://localserverip/kimseak/repo-name.git
```

Move into project folder:

```bash
cd repo-name
```

---

# Project Setup

## Install CocoaPods

```bash
pod install
```

If CocoaPods is not installed:

```bash
sudo gem install cocoapods
```

---

## Open Workspace

```bash
open YourProject.xcworkspace
```

> Important:
>
> Always open `.xcworkspace`
>
> Do not open `.xcodeproj` when using CocoaPods.

---

## Resolve Swift Package Manager (SPM)

In Xcode:

```text
File → Packages → Resolve Package Versions
```

Or wait for Xcode to automatically resolve packages.

---

# Git Workflow

## Check Current Branch

```bash
git branch
```

---

## Pull Latest Develop Branch

```bash
git checkout develop
git pull origin develop
```

---

## Create New Branch

Recommended naming convention:

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

Or add specific file:

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

## Create Merge Request

1. Open GitLab
2. Go to **Merge Requests**
3. Click **New Merge Request**
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
- Review files before pushing
- Use meaningful commit messages
- Keep branches focused on one feature or fix

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

## Git Status

```bash
git status
```

---

## List Branches

```bash
git branch
```

---

## Commit History

```bash
git log --oneline
```

---

## Pull Latest Code

```bash
git pull
```

---

## Push Code

```bash
git push
```

---

# Troubleshooting

## CocoaPods Error

```bash
pod repo update
pod install
```

---

## Clean Build Folder

```text
Shift + Command + K
```

---

## Remove Derived Data

```bash
rm -rf ~/Library/Developer/Xcode/DerivedData
```

---

# Author
Kimseak
