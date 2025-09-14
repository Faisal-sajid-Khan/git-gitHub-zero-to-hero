# Creating a GitHub Repository (CLI Method)

## Step 1: Initialize Git
```bash
git init

Step 2: Add Files
git add .

Step 3: Commit Files
git commit -m "Initial commit"

Step 4: Create Repo on GitHub (CLI)
gh repo create git-github-zero-to-hero --public --description "Zero to Hero GitHub learning repo"


Step 5: Push Code
git branch -M main
git remote add origin https://github.com/<your-username>/git-github-zero-to-hero.git
git push -u origin main
