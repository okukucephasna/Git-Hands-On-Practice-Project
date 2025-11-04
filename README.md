# 🧠 Git Hands-On Practice Project

This project will help you **practice Git commands** in a realistic, hands-on way.
You’ll build a simple text-based repository to track your personal learning notes while mastering Git.

---

## 🗂️ Project: Personal Notes Tracker

You’ll create a simple repository to manage and version-control your personal notes.

---

### 🧩 Step 1: Initialize a Repository

```bash
# Create a project folder
mkdir notes-tracker
cd notes-tracker

# Initialize a Git repository
git init
```

---

### 📝 Step 2: Add Your First File

```bash
# Create your first notes file
echo "Day 1: Learning Git basics" > notes.txt

# Stage and commit
git add notes.txt
git commit -m "Initial commit: added notes.txt"
```

---

### 🌿 Step 3: Create and Switch Branches

```bash
# Create a new branch
git branch add-more-notes

# Switch to that branch
git checkout add-more-notes

# Add new content
echo "Day 2: Practiced git branch and git checkout" >> notes.txt

# Commit the changes
git add notes.txt
git commit -m "Added more notes in add-more-notes branch"
```

---

### 🔀 Step 4: Merge Branches

```bash
# Go back to main branch
git checkout main

# Merge the branch changes
git merge add-more-notes
```

---

### ⚠️ Step 5: Create a Merge Conflict

1. On the `main` branch, edit a line in `notes.txt`
2. On the `add-more-notes` branch, edit the **same** line differently
3. Try merging them again — Git will raise a **merge conflict**

```bash
# After resolving manually:
git add notes.txt
git commit -m "Resolved merge conflict in notes.txt"
```

---

### ☁️ Step 6: Push to GitHub

```bash
# Create a new repository on GitHub called notes-tracker

# Link your local repo to GitHub
git remote add origin https://github.com/<your-username>/notes-tracker.git
git branch -M main
git push -u origin main
```

---

### 🧠 Step 7: Keep Practicing

Try these commands to deepen your understanding:

```bash
git log --oneline
git diff
git stash
git revert <commit-id>
git tag v1.0
```
Use **meaningful commit messages**:
* ✅ What changed?
* ✅ Why was it changed?
---
### 💡 Pro Tip
As you read Git tutorials or books, don’t just skim examples —
**type every command yourself**, modify them slightly, and observe how Git responds.
That habit builds *real understanding*.

---

Would you li
