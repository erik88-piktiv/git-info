# Get info

- `git branch` shows a list of all branches.
- `git log [--oneline]` shows a list of all recent commits.
- `git show [commit]` shows the contents of a commit.
- `git status` shows the uncommited changes.

# Create commit

- `git add [path]` puts a file into staging.
- `git add .` puts all modified files into staging.
- `git commit -m "meddelande"` Creates a new commit of all files in staging, with message "meddelande"

- `git cherry-pick [commit]` takes a commit from another branch, and copies it into the current branch.

# Branching

- `git switch [branch-name]` checkout the branch (i.e. moved HEAD to the branch)
- `git branch -D [branch-name]` removes the branch.

# Undo

- `git restore .` restores all changed files back to last commit.
- `git revert [commit]` creates an anti-commit which undos the commit.
- `git reset [commit]` Removes all commits from HEAD back to the selected commit. Does not change the files, but marks them as changed.
- `git reset --hard [commit]` Removes all commits from HEAD back to the selected commit. **Removes the file changes** as well.

# rebase

- `git rebase [branch]` Rebases the current branch onto the selected branch.
- `git rebase -i [commit]` Brings up a prompt to rewrite the current branch's history down to the selected commit. **swag**
