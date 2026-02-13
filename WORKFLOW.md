# 🌊 Git & GitHub Workflow Guide

This guide outlines the standard development cycle for this project. Use these commands to keep your local work and GitHub repository in sync.

---

## 🚀 Daily Start: Synchronization
Before you start coding, always ensure you have the latest changes from the cloud.
```bash
git pull origin main
```

---

## 🛠️ Development Loop

### 1. Create a Feature Branch
Never work directly on `main`. Create a branch for your task:
```bash
git checkout -b feature/your-feature-name
```

### 2. Check Your Changes
See what files you've modified:
```bash
git status
```

### 3. Save Your Progress (Commit)
Stage and commit your changes with a descriptive message:
```bash
git add .
git commit -m "feat: brief description of what you did"
```

---

## ☁️ Daily Wrap-up: Backup to GitHub
When you're done for the day or finished a feature, push your branch:
```bash
git push origin feature/your-feature-name
```

---

## 🏁 Merging Changes
Once your feature is complete on GitHub:
1. Open a **Pull Request (PR)** on GitHub.com.
2. Merge the PR.
3. Locally, clean up and move back to the main track:
```bash
git checkout main
git pull origin main
```

> **Pro Tip:** Commit small, logical chunks of work. It makes finding bugs much easier later!
