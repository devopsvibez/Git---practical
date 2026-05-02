# Git Practical Demo 🚀

This project demonstrates a complete Git workflow for beginners.

It covers:
- Git setup
- First commit
- Push to GitHub
- Branching
- Merge conflict
- Conflict resolution

---

## Prerequisites

- Git installed
- GitHub account

Check Git version:
git --version

Configure your details:
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

---

## Step 1: Create Project

- mkdir git-demo
 - cd git-demo
- git init

---

## Step 2: Create File & Commit

- echo "Version 1" > app.txt
- add app.txt
- git status
- git commit -m "Initial commit"

---

## Step 3: Connect to GitHub

Create a repository on GitHub (example: Git-practical)

- git remote add origin <YOUR_REPO_URL>
- git branch -M main
- git push -u origin main

---

## Authentication (if required)

Use GitHub Personal Access Token instead of password.

Steps:
GitHub → Settings → Developer Settings → Personal Access Tokens  
Generate token → Select scope: repo  

Use:
Username → your GitHub username  
Password → your token  

---

## Step 4: Create Branch

git checkout -b feature-update

---

## Step 5: Update File in Feature Branch

- echo "Version 2 - feature" > app.txt
- git add app.txt
- git commit -m "Feature update"
- git push origin feature-update

---

## Step 6: Switch to Main Branch

git checkout main

---

## Step 7: Make Change in Main

- echo "Version 2 - main" > app.txt
- git add app.txt
- git commit -m "Main update"

---

## Step 8: Merge (Conflict Happens)

git merge feature-update

You will see:

<<<<<<< HEAD
Version 2 - main
=======
Version 2 - feature
>>>>>>> feature-update

---

## Step 9: Resolve Conflict

Replace file content with:

Version 2 - resolved

Then run:

- git add app.txt
- git commit -m "Resolved conflict"

---

## Step 10: Push Final Changes

git push

---

## Result

You have successfully completed:
- Git initialization
- Commit and push
- Branching
- Merge conflict creation
- Conflict resolution

Merge conflicts are normal in real projects.

---

devopsvibez 🚀
