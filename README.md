#!/bin/bash

# Configure Git (run once)
git config --global user.name "kowsick"
git config --global user.email "kowsickkowsick37@gmail.com"

# Verify Git configuration
git config --list

# Create a new project folder
mkdir Mission DHONI
cd Mission DHONI || exit

# Initialize Git repository
git init
# Create a README file
echo "Mission DHONI" > README.md

# Add all files to the staging area
git add .

# Commit the files
git commit -m "Initial commit"

# Rename the default branch to main
git branch -M main

# Add the GitHub remote repository
git remote add origin https://github.com/kowsick/Mission DHONI.git

# Push the project to GitHub
git push -u origin main

echo "Project has been successfully pushed to GitHub!"