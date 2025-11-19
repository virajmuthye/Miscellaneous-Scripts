#!/bin/bash
cat > README.md << 'EOF'
# GitHub Tutorial for Beginners

Welcome to this GitHub tutorial! This guide will walk you through the basics of using GitHub, from setting up your account to collaborating on projects.

---

## Table of Contents

1. [What is Git and GitHub?](#what-is-git-and-github)  
2. [Setting Up Your Environment](#setting-up-your-environment)  
3. [Creating a Repository](#creating-a-repository)  
4. [Cloning a Repository](#cloning-a-repository)  
5. [Making Changes and Committing](#making-changes-and-committing)  
6. [Pushing Changes to GitHub](#pushing-changes-to-github)  
7. [Branching and Merging](#branching-and-merging)  
8. [Pull Requests](#pull-requests)  
9. [Collaborating on GitHub](#collaborating-on-github)  
10. [Additional Resources](#additional-resources)  

---

## What is Git and GitHub?

- **Git** is a version control system that helps you track changes in your files over time.  
- **GitHub** is an online platform that hosts Git repositories and allows collaboration.  

Think of Git as the engine, and GitHub as the platform that lets you share and collaborate with others.

---

## Setting Up Your Environment

1. **Install Git**  
   - Windows: https://git-scm.com/download/win  
   - macOS: brew install git  
   - Linux: sudo apt install git  

2. **Set Up Git**  
   Open your terminal or command prompt and type:  
   git config --global user.name "Your Name"  
   git config --global user.email "your.email@example.com"  

3. **Check Installation**  
   git --version

---

## Creating a Repository

1. Go to https://github.com/ and log in.  
2. Click the + icon in the top-right corner -> New repository.  
3. Enter a Repository Name, optional description, and choose Public or Private.  
4. Click Create repository.

---

## Cloning a Repository

git clone https://github.com/username/repository-name.git  
cd repository-name

---

## Making Changes and Committing

1. Open or create a file in your repository.  
2. Add the changes to the staging area:  
   git add filename  
   Or add all files:  
   git add .  
3. Commit your changes with a message:  
   git commit -m "Your commit message"

---

## Pushing Changes to GitHub

git push origin main

> Note: Replace main with your branch name if different.

---

## Branching and Merging

git checkout -b feature-branch  
git checkout main  
git merge feature-branch

---

## Pull Requests

git push origin feature-branch  
Create pull request via GitHub UI  
Merge after review

---

## Collaborating on GitHub

- Fork a repository and clone locally  
- Make changes and submit a pull request  
- Use Issues to track bugs or feature requests

---

## Additional Resources

- https://docs.github.com/  
- https://git-scm.com/book/en/v2  
- https://lab.github.com/  

---

*This tutorial is beginner-friendly and ready to use for anyone starting with Git and GitHub.*
EOF

echo "README.md created successfully!"
