# hello-world
This repository is for practicing the GitHub Flow

# Walkthrough of "Create the Repository"

## 1. GUI Method (GitHub Website)

1. Go to [https://github.com](https://github.com) and sign in.
2. In the upper-right corner, click the **"+" icon** and select **"New repository"**.
3. In the **Repository name** field, type: `Name of the repo you want to create`.
4. In the **Description** field, type: `Short note about what the repo is about`
5. Choose the repository visibility:
   - Public: Anyone can see this repo.
   - Private: Only you and collaborators can see this repo.
6. Check the box: **Add a README file**.
7. Click the green **"Create repository"** button.

## 2. CLI Method (Command Line Interface)

```bash
# Create a local project folder and initialize Git
mkdir <repo-name> && cd <repo-name>
git init  # Initialize a new local Git repository

# Add a remote origin (replace <your-username> and <repo-name>)
git remote add origin https://github.com/<your-username>/<repo-name>.git

# Create a README file, add, commit, and push to GitHub
echo "# <repo-name>" > README.md
git add README.md
git commit -m "feat: initial commit with README"
git branch -M main  # Rename default branch to 'main' if needed
git push -u origin main

Note:
- Replace <your-username> with your GitHub username.
- Replace <repo-name> with the name of your repository.
- Make sure the repository is already created on GitHub before pushing.
