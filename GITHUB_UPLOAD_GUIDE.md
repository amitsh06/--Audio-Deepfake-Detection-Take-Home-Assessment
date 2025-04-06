# GitHub Upload Guide

This document provides step-by-step instructions for uploading this project to GitHub.

## Prerequisites

1. A GitHub account - Create one at [github.com](https://github.com) if you don't have one
2. Git installed on your computer - Download from [git-scm.com](https://git-scm.com/downloads)

## Step 1: Initialize Git Repository

Open a terminal/command prompt in your project directory and run:

```bash
git init
```

## Step 2: Add Files to Git

```bash
git add .
```

This adds all files to be tracked by Git, except those specified in the `.gitignore` file.

## Step 3: Commit Your Files

```bash
git commit -m "Initial commit"
```

## Step 4: Create a New Repository on GitHub

1. Go to [github.com](https://github.com) and log in
2. Click the '+' icon in the top-right corner and select 'New repository'
3. Name your repository (e.g., "audio-deepfake-detection")
4. Add a description (optional)
5. Choose public or private repository
   - Public: Anyone can see the repository, but you control who can commit
   - Private: You choose who can see and commit to the repository
6. Do NOT initialize the repository with a README, .gitignore, or license (we already have these)
7. Click 'Create repository'

## Step 5: Link Your Local Repository to GitHub

After creating the repository, GitHub will show commands to push an existing repository. Run these commands in your terminal:

```bash
git remote add origin https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git
git branch -M main
git push -u origin main
```

Replace `YOUR-USERNAME` and `REPOSITORY-NAME` with your GitHub username and the name you gave your repository.

## Step 6: Verify Upload

1. Refresh your GitHub repository page
2. You should see all your project files uploaded
3. The README_for_GitHub.md file will be displayed as the repository's README (you may want to rename it to README.md before pushing)

## Additional Tips

### Using GitHub Desktop

If you prefer a GUI over command line:
1. Download [GitHub Desktop](https://desktop.github.com/)
2. Use it to commit and push your repository

### Large Files

If you have large files (>100MB), consider using [Git LFS](https://git-lfs.github.com/) or keeping them out of the repository (they should already be excluded by the .gitignore file).

### Updating Your Repository

After making changes to your project, push them to GitHub with:

```bash
git add .
git commit -m "Description of changes"
git push
```

### Using the Correct README

Before pushing to GitHub, you may want to:

```bash
mv README_for_GitHub.md README.md
```

This will replace the current README with the GitHub-optimized version.