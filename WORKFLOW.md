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
git push -u origin HEAD
```

---

## 🏁 Merging Changes (The CLI Way)
Now that you have the GitHub CLI installed, you don't need to visit the website to merge!

1. **Create a Pull Request:**
   ```bash
   gh pr create --title "Your feature title" --body "What you did"
   ```
2. **Merge the PR:**
   ```bash
   gh pr merge --merge --delete-branch
   ```
3. **Sync back to Main:**
   ```bash
   git checkout main
   git pull origin main
   ```

---

## 🧹 Keeping it Clean: .gitignore
To prevent tracking "junk" files (like `.DS_Store` or `node_modules`), ensure you have a `.gitignore` file. I've created a basic one for you.

---

> **Pro Tip:** Commit small, logical chunks of work. It makes finding bugs much easier later!
