# Git & GitHub Quick Notes

## 1. Start Git

```bash
git init
```

Creates a Git repository in the project.

```bash
git branch -M main
```

Sets the main branch name to `main`.

---

## 2. Check Changes

```bash
git status
```

Shows the current branch and changed files.

---

## 3. Save Changes

```bash
git add .
```

Stages all changed files for the next commit.

```bash
git commit -m "Add home page"
```

Saves the staged changes as a commit.

---

## 4. Work with Branches

```bash
git branch
```

Shows available branches. `*` shows the current branch.

```bash
git checkout -b feature/sliders
```

Creates a new feature branch and switches to it.

```bash
git checkout main
```

Switches back to `main`.

---

## 5. GitHub

```bash
git push
```

Uploads local commits to GitHub.

```bash
git pull origin main
```

Gets the latest changes from GitHub.

---

## 6. Merge a Feature

```bash
git checkout main
git pull origin main
git merge feature/sliders
git push origin main
```

Merges the completed feature into `main` and updates GitHub.

---

## 7. Delete a Completed Branch

```bash
git branch -d feature/sliders
```

Deletes the local feature branch.

```bash
git push origin --delete feature/sliders
```

Deletes the feature branch from GitHub.

---

## My Basic Workflow

```text
main
 ↓
create feature branch
 ↓
work + test
 ↓
git add .
 ↓
git commit
 ↓
git push
 ↓
merge into main
 ↓
delete feature branch
```

### Remember

**Git** → tracks my code locally.

**GitHub** → stores and manages my repository online.
