# Git Cheat Sheet

A quick reference for common Git commands.

## Creating a Branch

### Create a New Branch
```shell
git branch new-branch-name
```

### Switch to the New Branch
```shell
git checkout new-branch-name
```

### Create and Switch to a New Branch in One Step
```shell
git checkout -b new-branch-name
```

## Staging Changes

### Stage All Changes
```shell
git add .
```

### Stage Specific File(s)
```shell
git add file1.txt file2.txt
```

## Creating a Commit

### Commit Staged Changes
```shell
git commit -m "Your commit message"
```

### Commit All Changes (Staged and Unstaged)
```shell
git commit -am "Your commit message"
```

## Pushing a Commit

### Push to Remote Repository
```shell
git push origin branch-name
```

## Checking the Status

### Check the Status of Your Repository
```shell
git status
```

## Reviewing History

### View Commit History
```shell
git log
```

### View Commit History in a Compact Format
```shell
git log --oneline
```

### View Changes in a Specific Commit
```shell
git show commit-hash
```

## Merging Changes

### Merge a Branch into the Current Branch
```shell
git merge branch-name
```

### Rebase the Current Branch onto Another Branch
```shell
git rebase branch-name
```

## Updating the Repository

### Update Local Repository with Remote Changes
```shell
git pull
```

### Fetch Remote Changes (Without Merging)
```shell
git fetch
```

## Removing Changes

### Discard Unstaged Changes
```shell
git checkout -- file.txt
```

### Reset to a Specific Commit
```shell
git reset --hard commit-hash
```

### Delete a Local Branch
```shell
git branch -d branch-name
```

### Delete a Remote Branch
```shell
git push origin --delete branch-name
```

## Configuration

### Configure Your Username
```shell
git config --global user.name "Your Name"
```

### Configure Your Email Address
```shell
git config --global user.email "youremail@example.com"
```

## Git Help

### Get Help on a Git Command
```shell
git help command
```

Replace placeholders like `new-branch-name`, `file1.txt`, `branch-name`, and `commit-hash` with your actual branch names, file names, and commit hashes.

Remember to customize the commit messages to describe your changes effectively.

For more detailed information on Git commands and options, you can refer to the official Git documentation using `git help` or visit [git-scm.com](https://git-scm.com/doc).
