# Git Workflow + Branching

## SkillAudit.ai DevOps Internship - Week 1

This repository demonstrates the Git workflow used in professional software development teams. The objective of this project is to understand Git branching strategies, Pull Requests, merge conflicts, conflict resolution, and rebasing.

---

## 📌 Internship Details

- **Organization:** SkillAudit.ai
- **Internship:** DevOps Internship
- **Week:** 1
- **Task:** Git Workflow + Branching

---

## 🎯 Objective

The main objectives of this task are:

- Learn Git branching workflow
- Create feature branches
- Create and merge Pull Requests
- Simulate and resolve merge conflicts
- Understand Git Rebase
- Maintain a clean commit history

---

## 🛠 Tools Used

- Git
- GitHub
- Visual Studio Code
- Ubuntu (WSL)

---

## 📂 Project Structure

```
git-workflow-demo/
│
├── README.md
├── app.txt
├── notes.txt
├── writeup.md
└── screenshots/
```

---

# Workflow Performed

## Step 1 – Repository Creation

- Created a new public GitHub repository.
- Cloned the repository locally.

Commands:

```bash
git clone <repository-url>
cd git-workflow-demo
```

---

## Step 2 – Initial Commit

Created project files.

```text
README.md
app.txt
```

Committed the initial project.

```bash
git add .
git commit -m "Initial project setup"
git push -u origin main
```

---

## Step 3 – Feature Branch

Created a feature branch.

```bash
git checkout -b feature/login
```

Added login feature.

Committed changes.

```bash
git add .
git commit -m "Add login feature"
```

Pushed branch.

```bash
git push origin feature/login
```

---

## Step 4 – Pull Request

Created a Pull Request on GitHub.

Merged the Pull Request into the **main** branch.

---

## Step 5 – Merge Conflict

Created another feature branch.

```bash
git checkout -b feature/dashboard
```

Modified the same file on both branches.

Merged main into feature branch.

```bash
git merge main
```

Git produced a merge conflict.

Resolved the conflict manually.

Committed the resolution.

```bash
git add app.txt
git commit -m "Resolve merge conflict"
```

---

## Step 6 – Git Rebase

Created another feature branch.

```bash
git checkout -b feature/profile
```

Updated the main branch.

Rebased the feature branch.

```bash
git rebase main
```

Pushed the rebased branch.

```bash
git push --force-with-lease origin feature/profile
```

---

# What I Learned

During this task I learned how software development teams collaborate using Git.

### Git Branching

Branches allow developers to work independently without affecting the main codebase.

### Pull Requests

Pull Requests are used for code review before merging changes into the main branch.

### Merge Conflicts

Merge conflicts occur when two branches modify the same section of a file.

The conflict must be resolved manually before Git can complete the merge.

### Git Rebase

Rebase moves feature branch commits to the latest commit of the main branch.

Unlike merge, rebase creates a cleaner and more linear commit history.

---

# Git Commands Used

```bash
git clone <repository-url>

git status

git branch

git checkout -b feature/login

git add .

git commit -m "Initial project setup"

git commit -m "Add login feature"

git push origin feature/login

git checkout main

git pull origin main

git merge main

git rebase main

git log --oneline --graph --all

git push --force-with-lease
```

---

# Screenshots

The **screenshots** folder contains:

- Repository Creation
- Initial Commit
- Feature Branch Creation
- Pull Request
- Pull Request Merge
- Merge Conflict
- Conflict Resolution
- Git Rebase
- Final Commit History
- Final Repository

---

# Final Outcome

Successfully completed the following tasks:

- Repository Creation
- Feature Branching
- Pull Request Creation
- Pull Request Merge
- Merge Conflict Resolution
- Git Rebase
- Clean Git Commit History

