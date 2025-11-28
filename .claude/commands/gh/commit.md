---
allowed-tools: Bash
description: Analyze changes, generate commit message, and push to GitHub
---

## Task

Analyze the current git changes, automatically generate a commit message following Conventional Commits format, commit the changes, and push to the remote repository.

## Workflow

### Step 1: Analyze Changes

First, check the current git status and changes:
- Run `git status` to see modified, added, and deleted files
- Run `git diff --cached` to see staged changes (if any)
- Run `git diff` to see unstaged changes

### Step 2: Generate Commit Message

Based on the changes, generate a commit message following **Conventional Commits** format:

**Format**: `<type>: <description>`

**Types**:
- `feat`: New feature or functionality
- `fix`: Bug fix
- `docs`: Documentation changes only
- `refactor`: Code refactoring (no functionality change)
- `style`: Code style changes (formatting, whitespace)
- `test`: Adding or updating tests
- `chore`: Maintenance tasks, dependencies, config

**Guidelines**:
- Keep description concise (50 chars or less preferred)
- Use present tense ("add" not "added")
- Don't capitalize first letter after type
- No period at the end

**Examples**:
- `feat: add user authentication system`
- `fix: resolve login validation error`
- `docs: update installation guide`
- `refactor: simplify database queries`

### Step 3: Commit and Push

Execute the following:
1. Stage all changes: `git add .`
2. Commit with generated message: `git commit -m "<generated-message>"`
3. Push to remote: `git push`

### Step 4: Error Handling

If errors occur:

**Conflict or uncommitted changes**:
- Stash current changes: `git stash`
- Pull latest: `git pull --rebase`
- Pop stash: `git stash pop`
- Retry commit and push

**No changes to commit**:
- Inform user that working directory is clean
- No action needed

**Push rejected (non-fast-forward)**:
- Pull latest changes first: `git pull --rebase`
- Retry push

## Important Notes

- **No confirmation required** - automatically commit and push
- Always use Conventional Commits format
- Analyze ALL changes to create accurate commit message
- Handle errors gracefully with automatic retry
- Always push after successful commit

## Example Output

After analyzing changes and committing, show:
```
✓ Analyzed changes: 5 files modified, 2 files added
✓ Generated commit message: "feat: add GitHub workflow commands"
✓ Committed changes
✓ Pushed to remote: origin/main
```
