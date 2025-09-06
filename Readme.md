# Git Remote Repository Commands

This document lists commonly used Git commands for working with remote
repositories and pulling changes.

## 1. Configure Remote Repository

``` bash
# Add a new remote repository
git remote add origin <repository_url>

# Verify remote repositories
git remote -v
```

## 2. Clone a Repository

``` bash
# Clone an existing remote repository
git clone <repository_url>
```

## 3. Fetch Changes

``` bash
# Fetch updates from remote (does not merge)
git fetch origin

# Fetch all branches from all remotes
git fetch --all
```

## 4. Pull Changes

``` bash
# Pull changes from remote default branch (usually main or master)
git pull origin main

# Pull changes from a specific branch
git pull origin <branch_name>

# Pull and rebase instead of merge
git pull --rebase origin <branch_name>
```

## 5. Branch Management

``` bash
# Create and switch to a new branch
git checkout -b <branch_name>

# Switch to an existing branch
git checkout <branch_name>

# Track a remote branch locally
git checkout --track origin/<branch_name>
```

## 6. Push Changes

``` bash
# Push commits to remote repository
git push origin <branch_name>

# Push and set upstream branch
git push -u origin <branch_name>
```

## 7. Sync Forked Repository

``` bash
# Add upstream repository (original repo)
git remote add upstream <upstream_repo_url>

# Fetch latest changes from upstream
git fetch upstream

# Merge upstream changes into local branch
git merge upstream/main

# Or rebase with upstream
git rebase upstream/main
```

------------------------------------------------------------------------

✅ Use `git status` and `git log` frequently to check the state of your
repo.
