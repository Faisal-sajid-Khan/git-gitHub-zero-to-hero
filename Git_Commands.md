         ######### Git Commands in Different Scenarios ############

## 🔹 Basic Setup
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

1 Starting a Repository
git init
git clone https://github.com/username/repo.git

2 Staging & Committing
git add file.txt
git add .
git commit -m "Your commit message"

3 Branching
git branch                # List branches
git branch new-feature    # Create branch
git checkout new-feature  # Switch branch
git checkout -b feature-x # Create + switch
git branch -d branch-name # Delete branch

4 Merging & Rebasing
git merge branch-name
git rebase branch-name

5 Remote Repositories
git remote add origin https://github.com/username/repo.git
git remote -v
git push -u origin main
git pull origin main
git fetch origin

6 Undoing Changes
git reset file.txt                # Unstage file
git reset --hard HEAD             # Reset everything to last commit
git checkout -- file.txt          # Discard changes in file
git revert <commit-hash>          # Undo a commit (safe)

7 Viewing History
git log
git log --oneline --graph --all
git status
git diff

8 Tagging
git tag v1.0.0
git tag -a v1.0.0 -m "Version 1.0"
git push origin v1.0.0

9 Deleting
git rm file.txt
git push origin --delete branch-name

10 Stash (Save Work Temporarily)
git stash
git stash list
git stash apply stash@{0}

          ######Real-World Git Workflow (Feature Branch → PR → Merge → Delete)#######

Step 1: Clone the repo
git clone https://github.com/username/repo.git
cd repo

Step 2: Create a feature branch
git checkout -b feature-login

Step 3: Work on your changes
git add .
git commit -m "Added login feature"

Step 4: Push branch to GitHub
git push -u origin feature-login

Step 5: Open a Pull Request (PR)
Go to GitHub → Open PR from feature-login → main.

Step 6: Review & Merge
After approval, merge the PR into main.

Step 7: Sync local main
git checkout main
git pull origin main

Step 8: Delete feature branch
git branch -d feature-login
git push origin --delete feature-login

