#!/bin/bash

# Replace these variables with your own repository URL and credentials
REPO_URL="https://github.com/yourusername/your-repo.git"
USERNAME="yourusername"
PASSWORD="yourpassword"

# Initialize a new Git repository
git init

# Create a README file
echo "# My Project" > README.md

# Add the README file to the repository
git add .

# Commit the changes
git commit -m "Initial commit"

# Push the commits to the remote repository
git remote add origin "$REPO_URL"
git push -u origin master
