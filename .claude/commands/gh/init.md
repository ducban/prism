---
allowed-tools: Bash
description: Initialize git repository and push to remote
---

## Task

Initialize a new git repository, commit all files, and push to the remote repository.

**Repository URL**: `$ARGUMENTS`

## Steps

1. **Initialize git repository**:
   - Run `git init`
   - Add all files to staging
   - Create initial commit with message "Project's docs and plan initiated"

2. **Setup remote and push**:
   - Rename branch to `main`
   - Add remote origin with the provided URL
   - Push to remote

## Important

- Ensure the repository URL is valid
- If git is already initialized, skip `git init`
- If remote already exists, update it instead of adding
- Handle any errors gracefully and inform the user

## Commands to Execute

```bash
# Initialize repository
git init

# Stage all files
git add .

# Initial commit
git commit -m "Project's docs and plan initiated"

# Rename to main branch
git branch -M main

# Add remote origin
git remote add origin $ARGUMENTS

# Push to remote
git push -u origin main
```

If any step fails, report the error and provide suggestions for fixing it.
