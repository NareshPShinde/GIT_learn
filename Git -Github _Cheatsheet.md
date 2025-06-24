Git Cheatsheet
--------------

This cheat sheet features the foremost important and commonly used Git commands for straightforward reference. It also takes into care some of the high-level concepts of Git. 

Uses of Git
-----------

Git is the most widely used version control system because of the various absolute benefits offered by it :

*   Git is well known for providing the best performance when it comes to the different distributed version control systems. The operations of branching, committing, and merging are all optimized for a far better performance than other systems.
    
*   Git is employed to maintain the history and keep track of the changes in the source code files.
    
*   Git helps in independent collaborative working and allows multiple developers to collaborate and share their work.
    
*   One of Git's main benefits of Git is that it supports working in offline mode without having internet connectivity, So, just in case you have internet connectivity issues, it won't be affecting your work at all.
    
*   Git gives you the power to undo almost any command or action.
    
*   It is known to be a non-linear development due to its thousands of parallel branches.
    
*   It is scalable and provides the user to work in a distributed environment.
    
*   Git has an intermediate stage called the **"staging area"** where commits are often formatted, edited, and modified before completing the commit.
    
*   It is free and open source and allows the creation of a backup.
    
*   This is an industry-standard as most IDEs support Git.
    
*   Git is meant to ensure the safety and integrity of versioned content.
    
*   Each command in Git only takes some seconds to run and output results, so it saves a lot of developers' effort and time.

# 🧠 Git & GitHub Cheat Sheet

A concise and comprehensive cheat sheet for mastering Git commands and GitHub workflows.

---

## ⚙️ Git Configuration
```bash
git config --list                    # View all Git config
git config --get user.email         # Get current Git email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global alias.co checkout  # Shortcut alias
```

---

## 📁 Repository Initialization & Cloning
```bash
git init                             # Initialize a Git repo
git clone <repo_url>                # Clone an existing repo
git clone -b <branch> <url>         # Clone specific branch
git clone --bare <url>              # Clone a bare repo
```

---

## 📝 Staging & Committing Changes
```bash
git status                           # Show file status
git add <file>                       # Stage single file
git add .                            # Stage all changes
git commit -m "message"              # Commit staged files
git commit -am "message"             # Stage and commit tracked files
git commit --amend                   # Modify last commit
```

---

## 🧾 Diff & History
```bash
git diff                             # Unstaged changes
git diff --staged                    # Staged changes
git log                              # Commit history
git log --oneline                    # One line per commit
git log --graph                      # Branch structure
git show                             # Show specific commit
git reflog                           # History of HEAD
```

---

## 🌿 Branching & Merging
```bash
git branch                           # List branches
git branch <branch>                 # Create new branch
git checkout <branch>               # Switch branch
git checkout -b <branch>            # Create and switch
git merge <branch>                  # Merge into current
git branch -d <branch>              # Delete merged branch
git branch -D <branch>              # Force delete branch
```

---

## 🔄 Undo & Reset
```bash
git revert <commit>                 # Revert a commit
git reset <file>                    # Unstage file
git reset --hard HEAD~1             # Reset to previous commit
git rm <file>                       # Delete file from working & staging
git rm --cached <file>              # Remove from staging only
```

---

## 🧳 Stashing
```bash
git stash                            # Save changes
git stash list                       # Show stashes
git stash apply                      # Re-apply stash
git stash pop                        # Apply and remove
git stash drop                       # Delete stash
```

---

## ✨ Rebase & Cherry-Pick
```bash
git rebase <branch>                 # Reapply commits over another base
git rebase -i HEAD~N                # Interactive rebase
git cherry-pick <commit>            # Apply single commit
```

---

## 🌐 GitHub Specific
```bash
git remote -v                        # Show remotes
git remote add origin <url>         # Link to GitHub repo
git push -u origin <branch>         # Push new branch
git pull origin <branch>            # Pull latest changes
git fetch origin                    # Fetch from GitHub
git push origin --delete <branch>   # Delete remote branch
```

---

## 🔐 GitHub SSH Setup
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
# Copy public key and add to GitHub Settings > SSH Keys
```

---

## ✅ Best Practices
- Use `.gitignore` to exclude files
- Always pull before pushing
- Write meaningful commit messages
- Use branches for features/fixes
- Keep your main branch clean and deployable

---

> ✨ Keep this cheat sheet handy for efficient Git & GitHub development!
