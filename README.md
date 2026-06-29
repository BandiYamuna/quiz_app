# Git Practice - Ecommerce Project

## Overview

This repository was created to practice basic Git and GitHub commands, including repository initialization, file tracking, committing changes, viewing history, and pushing code to GitHub.

## Git Commands Practiced

### 1. Create a Project

```bash
mkdir ecommerce
cd ecommerce
```

### 2. Initialize Git Repository

```bash
git init
```

### 3. Check Repository Status

```bash
git status
```

### 4. Add Files to Staging Area

Add a single file:

```bash
git add index.html
```

Add all files:

```bash
git add .
```

### 5. Commit Changes

```bash
git commit -m "footer about add"
```

Second commit:

```bash
git commit -m "add test file"
```

### 6. View Commit History

```bash
git log
```

### 7. View Commit Details

```bash
git show <commit-id>
```

### 8. Add Remote Repository

```bash
git remote add origin https://github.com/BandiYamuna/quiz_app.git
```

### 9. Rename Branch

```bash
git branch -M main
```

### 10. Push Code to GitHub

First push:

```bash
git push origin main
```

Set upstream branch:

```bash
git push -u origin main
```

### 11. Verify Remote Repository

```bash
git remote -v
```

## Files Created

* index.html
* about.html
* footer.html
* test.txt

## Git Concepts Learned

* Creating a local Git repository
* Tracking files using `git add`
* Understanding untracked, staged, and committed files
* Creating commits with meaningful messages
* Viewing commit history using `git log`
* Inspecting commit changes using `git show`
* Connecting a local repository to GitHub
* Renaming the default branch to `main`
* Pushing code to a remote repository
* Setting the upstream branch using `git push -u`
* Checking remote repository details using `git remote -v`

## Common Mistake Encountered

Incorrect command:

```bash
git commit -M "add test file"
```

Error:

```
error: unknown switch `M'
```

Correct command:

```bash
git commit -m "add test file"
```

## Outcome

Successfully created a local Git repository, committed project files, connected the repository to GitHub, and pushed the project to the remote repository while learning the complete basic Git workflow.



<img width="1603" height="972" alt="Screenshot 2026-06-30 001329" src="https://github.com/user-attachments/assets/ecd4e022-1794-4701-a59d-b692dded3aef" />
<img width="1913" height="1027" alt="Screenshot 2026-06-30 001353" src="https://github.com/user-attachments/assets/c31e9800-bb56-4cc9-a621-b33edf66ced0" />

