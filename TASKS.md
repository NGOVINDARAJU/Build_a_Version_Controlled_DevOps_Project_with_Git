# DevOps Assignment: Version-Controlled Project with Git

## Project Overview
This project demonstrates Git best practices for version control including:
- Branching (main, dev, feature)
- Pull requests (PR) workflow
- Commit history with proper messages
- Tagging releases
- Documentation using markdown

---

## Step-by-Step Process

### Step 1 — Git Setup
- Installed Git on local machine.
- Configured Git with name and email:
  ```bash
  git config --global user.name "Govindaraju"
  git config --global user.email "your.email@example.com"
### Step 2 — Initialize Repository
- Created project folder devops-project.
- Initialized Git repository:
  ```bash
  git init
  git status
### Step 3 — Add README.md and .gitignore
- Created README.md with project title.
- Created .gitignore to exclude IDE/build files.
- Committed changes:
  ```bash
  git add README.md .gitignore
  git commit -m "chore: initial commit - add README and .gitignore"
### Step 4 — Push to GitHub
- Created GitHub repository Build_a_Version_Controlled_DevOps_Project_with_Git
- Connected local repo to GitHub:
  ```bash
  git remote add origin https://github.com/NGOVINDARAJU/Build_a_Version_Controlled_DevOps_Project_with_Git.git
  git branch -M main
  git push -u origin main
- Used Personal Access Token (PAT) for authentication.
### Step 5 — Branching
- Created dev branch:
  ```bash
  git checkout -b dev
  git push -u origin dev
- Created feature branch feature/demo-change from dev:
  ```bash
  git checkout -b feature/demo-change
  git push -u origin feature/demo-change
### Step 6 — Pull Request Workflow
- Made changes in feature/demo-change (added demo section in README).
- Opened PR feature → dev, resolved merge conflict, merged successfully.
- Opened PR dev → main, merged changes into main.
### Step 7 — Tagging a Release
- Switched to main branch:
  ```bash
  git checkout main
  git pull origin main
- Created annotated tag for release:
  ```bash
  git tag -a v0.1.0 -m "v0.1.0 - initial release"
  git push origin v0.1.0
- Verified tag on GitHub.
### Branches Overview
- main → Production-ready code
- dev → Development branch for testing
- feature/demo-change → Feature branch for small changes
  
  

  
