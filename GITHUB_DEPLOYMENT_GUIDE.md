# GitHub Pages Deployment Guide

Follow these step-by-step instructions to push your portfolio website to GitHub and enable GitHub Pages hosting.

## Prerequisites
- Git installed on your system
- GitHub account
- Your repository URL: `https://github.com/aadish247/Portfolio-Website.git`

## Step 1: Open Terminal/Command Prompt
Open PowerShell or Command Prompt in your portfolio website directory:
```
cd "c:\Users\Aadish\py\Portfolio website"
```

## Step 2: Initialize Git Repository
If not already initialized:
```
git init
```

## Step 3: Add All Files
Add all your portfolio files to git:
```
git add .
```

## Step 4: Commit Your Changes
```
git commit -m "Initial portfolio website with all updates"
```

## Step 5: Add Remote Repository
```
git remote add origin https://github.com/aadish247/Portfolio-Website.git
```

## Step 6: Push to GitHub
For the first push:
```
git push -u origin main
```

If your default branch is 'master' instead of 'main':
```
git push -u origin master
```

## Step 7: Enable GitHub Pages
1. Go to your repository on GitHub: https://github.com/aadish247/Portfolio-Website
2. Click on **Settings** tab
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Select **main** (or **master**) branch and **/ (root)** folder
6. Click **Save**

## Step 8: Access Your Live Website
Your website will be available at:
```
https://aadish247.github.io/Portfolio-Website/
```

## Troubleshooting

### If you get "main branch not found" error:
```
git branch -M main
git push -u origin main
```

### If you have authentication issues:
- Use GitHub Personal Access Token instead of password
- Or use GitHub Desktop for easier authentication

### To update your website later:
```
git add .
git commit -m "Update description"
git push
```

## Verify Everything Works
After pushing, wait 5-10 minutes for GitHub Pages to deploy, then visit your URL to verify everything works correctly.