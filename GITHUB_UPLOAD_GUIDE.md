# GitHub Upload Guide

## Prerequisites

1. **Install Git** (if not already installed):
   - Download from: https://git-scm.com/download/win
   - Install with default settings
   - Restart your terminal/IDE after installation

2. **GitHub Account**: Make sure you're logged into GitHub

## Steps to Upload Project

### Option 1: Using Command Line (Recommended)

1. **Open Terminal/PowerShell** in the project directory:
   ```
   C:\Users\Talek\Desktop\neha\ReNDR nextjs\nation-one-debt-relief
   ```

2. **Initialize Git** (if not already initialized):
   ```bash
   git init
   ```

3. **Add all files**:
   ```bash
   git add .
   ```

4. **Create .gitignore** (if not exists) to exclude unnecessary files:
   ```bash
   echo "node_modules/" > .gitignore
   echo ".next/" >> .gitignore
   echo ".env.local" >> .gitignore
   echo ".env" >> .gitignore
   echo ".DS_Store" >> .gitignore
   ```

5. **Commit the files**:
   ```bash
   git commit -m "Initial commit: Nation One Debt Relief website"
   ```

6. **Add the remote repository**:
   ```bash
   git remote add origin https://github.com/neha-bigdrops/Re_NDR.git
   ```

7. **Rename branch to main** (if needed):
   ```bash
   git branch -M main
   ```

8. **Push to GitHub**:
   ```bash
   git push -u origin main
   ```

### Option 2: Using GitHub Desktop

1. Download GitHub Desktop: https://desktop.github.com/
2. Sign in with your GitHub account
3. Click "File" > "Add Local Repository"
4. Navigate to: `C:\Users\Talek\Desktop\neha\ReNDR nextjs\nation-one-debt-relief`
5. Click "Publish repository"
6. Select the repository: `neha-bigdrops/Re_NDR`
7. Click "Publish Repository"

### Option 3: Using VS Code

1. Open the project in VS Code
2. Open the Source Control panel (Ctrl+Shift+G)
3. Click "Initialize Repository"
4. Stage all files (click + next to "Changes")
5. Commit with message: "Initial commit"
6. Click "..." menu > "Remote" > "Add Remote"
7. Enter: `https://github.com/neha-bigdrops/Re_NDR.git`
8. Click "Publish Branch"

## Important Notes

- Make sure to create a `.gitignore` file to exclude:
  - `node_modules/`
  - `.next/`
  - `.env` files
  - Build artifacts

- If you encounter authentication issues, you may need to:
  - Use a Personal Access Token instead of password
  - Set up SSH keys
  - Use GitHub Desktop for easier authentication

## Troubleshooting

If you get "repository not found" error:
- Make sure the repository exists at: https://github.com/neha-bigdrops/Re_NDR
- Check that you have write access to the repository

If you get authentication errors:
- Use GitHub Desktop for easier setup
- Or set up a Personal Access Token: https://github.com/settings/tokens

