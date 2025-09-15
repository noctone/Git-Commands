# Git Practice Log – [15th Sep 2025]

## Overview
Today, I practiced essential Git operations to strengthen my workflow and build confidence with a live repository.  
The focus was on: staging, committing, amending, branching, pushing, and merging.

---

## Work Done

### 1. Checked repository status
- Verified current branch, staged and unstaged changes using:
git status
- Ensured I was on the correct branch before making any changes.

### 2. Staged changes intentionally
- Added specific files to commits using:
git add <file>
- Avoided adding unnecessary or temporary files.

### 3. Committed with clear messages
- Committed changes with descriptive messages:
git commit -m "Descriptive commit message"
- Practiced concise and meaningful messages to improve history readability.

### 4. Amended the last commit
- Added a forgotten file:
git add fix_bug.py
- Amended the last commit to include new changes:
git commit --amend
- Updated the commit message to reflect the changes.

### 5. Worked with branches
- Created and switched to a feature branch:
git checkout -b feature/git-practice
- Ensured work was isolated from main.

### 6. Pushed changes safely
- First-time push of the branch to remote:
git push -u origin feature/git-practice

### 7. Merged feature branch into main
- Switched to main:
git checkout main
- Pulled latest changes from remote:
git pull origin main
- Merged feature branch, allowing unrelated histories:
git merge feature/git-practice --allow-unrelated-histories
- Resolved conflicts manually, then staged and committed:
git add <resolved-file>
git commit
- Pushed updated main branch:
git push origin main
> ✅ Successfully merged feature branch into main, handling unrelated histories.

---

## Key Learnings
- Always check git status before making changes.  
- Stage only the files you intend to commit.  
- Amend commits to keep history clean before pushing.  
- Feature branches protect main and simplify merges.  
- --allow-unrelated-histories fixes merges with no shared ancestor.  
- Resolve conflicts manually, then stage and commit.

---

## Next Steps
- Practice git push --force-with-lease safely.  
- Learn to squash multiple commits using git rebase -i.  
- Refine commit messages and branch naming conventions.

---

## Troubleshooting: "fatal: refusing to merge unrelated histories"
- Occurs when Git detects no common ancestor between branches.  
- Fix by using:
git merge <branch-name> --allow-unrelated-histories
- Always backup your branch first:
git branch backup-feature
- Resolve conflicts manually, stage, then commit.

---

## Recommended Workflow Summary
1. Check status → stage intentionally → commit clearly.  
2. Amend last commit only if necessary (pre-push).  
3. Work on feature branches → push safely.  
4. Merge branches (--allow-unrelated-histories if needed) → resolve conflicts.  
5. Backup before risky commands (force push, reset, etc.).

