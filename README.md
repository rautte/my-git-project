# My Git Project
## Updated README on main branch

# Step 1: Create directory and initialize Git repository
mkdir my-git-project
cd my-git-project
git init

# Step 2: Add and commit the initial file
echo "# My Git Project" > README.md
git add README.md
git commit -m "Initial commit"

# Step 3: Create a new branch
git checkout -b feature-branch

# Step 4: Make changes in feature-branch
echo "This is a new feature" > feature.txt
git add feature.txt
git commit -m "Added feature.txt"

# Step 5: Switch back to main and make changes
git checkout main
echo "## Updated README on main branch" >> README.md
git add README.md
git commit -m "Updated README on main branch"

# Step 6: Merge feature-branch into main
git merge feature-branch
    - Press ESC
    - Write ":wq" and press Enter to make the merge happen and get back to the CLI
    -  Write ":q!" and press Enter to stop the merge and get back to the CLI

# Step 7: Add GitHub remote and push to GitHub
git remote add origin https://github.com/your-username/my-git-project.git
git push -u origin main
git push -u origin feature-branch   # Optional: if you want to push feature-branch

