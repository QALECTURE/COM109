# Git Cheatsheet

Git is a version control tool. It helps developers save project history and manage changes.

## `git init`

```bash
git init
```

Creates a new Git repository in the current folder.

## `git status`

```bash
git status
```

Shows which files have changed and whether they are staged for commit.

## `git add .`

```bash
git add .
```

Stages all changed files so they are ready to be committed.

## `git commit -m`

```bash
git commit -m "Add homepage structure"
```

Creates a saved snapshot of your staged changes. The message should clearly describe what changed.

## `git branch`

```bash
git branch
```

Lists branches in the repository. A branch is a separate line of work.

Create a branch:

```bash
git branch feature-about-section
```

## `git remote add origin`

```bash
git remote add origin https://github.com/username/repository-name.git
```

Connects your local repository to a GitHub repository.

## `git push -u origin main`

```bash
git push -u origin main
```

Uploads your local commits to the `main` branch on GitHub. The `-u` option remembers the connection for future pushes.

## Common Workflow

```bash
git status
git add .
git commit -m "Describe the change"
git push
```

## Good Commit Messages

Good:

```text
Add contact form
Fix broken navigation link
Create portfolio homepage
```

Less useful:

```text
stuff
changes
final final version
```

