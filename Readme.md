# Git Practice Log – [15th Sep 2025]

## Overview
Today, I practiced essential Git operations to strengthen my workflow and build confidence with live repositories. The focus was on basic staging, committing, amending, branching, and safely pushing changes.

---

## Work Done

### 1. Checked repository status
- Used `git status` to verify:
  - Current branch
  - Unstaged changes
  - Staged changes
- Ensured I was working on the correct branch before making any changes.

### 2. Staged changes intentionally
- Selected specific files to include in commits using `git add <file>`.
- Avoided staging unnecessary or temporary files.

### 3. Committed with clear messages
- Committed changes using `git commit -m "Descriptive message"`.
- Practiced concise and meaningful commit messages to improve history readability.

### 4. Amended the last commit
- Staged a forgotten file: `git add fix_bug.py`.
- Amended the last commit using `git commit --amend`.
- Updated the commit message to reflect the newly included changes.

### 5. Worked with branches
- Created and switched to a feature branch for isolated work:  
  ```bash
  git checkout -b feature/git-practice
