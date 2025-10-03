# 🚀 AUTOMATED DEPLOYMENT SCRIPT FOR CODOZ TECHNOLOGY

## Your GitHub Credentials:
- **Email**: codoztech@gmail.com
- **Repository Name**: codoz-technology-website

## Step 1: Install Git (REQUIRED FIRST)

### Quick Install via Winget:
```powershell
winget install Git.Git
```

### Or Download Manually:
1. Go to: https://git-scm.com/download/win
2. Download "64-bit Git for Windows Setup"
3. Install with default settings
4. **RESTART your terminal/PowerShell after installation**

## Step 2: After Git Installation - Run These Commands

```bash
# Navigate to your project directory
cd "c:\Users\uk154\Downloads\final-file\skilline-landing-page-main"

# Configure Git (first time only)
git config --global user.name "Codoz Technology"
git config --global user.email "codoztech@gmail.com"

# Initialize repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit - Codoz Technology Website Launch"

# Add remote repository
git remote add origin https://github.com/codoztech/codoz-technology-website.git

# Push to GitHub
git push -u origin main
```

## Step 3: Create GitHub Repository

### Option A: Via GitHub CLI (after installing Git)
```bash
# Install GitHub CLI
winget install GitHub.cli

# Login to GitHub
gh auth login

# Create repository
gh repo create codoz-technology-website --public --description "Official Codoz Technology Website"

# Push code
git push -u origin main
```

### Option B: Manual Repository Creation
1. Go to https://github.com
2. Login with: codoztech@gmail.com
3. Click "+" → "New repository"
4. Name: `codoz-technology-website`
5. Description: "Official Codoz Technology Website - Digital Solutions Provider"
6. Set as **Public**
7. ✅ Add README file
8. Click "Create repository"

## Step 4: Enable GitHub Pages

1. Go to your repository: https://github.com/codoztech/codoz-technology-website
2. Click **Settings** tab
3. Scroll to **Pages** section (left sidebar)
4. Source: "Deploy from a branch"
5. Branch: "main"
6. Folder: "/ (root)"
7. Click **Save**

**Your site will be live at**: `https://codoztech.github.io/codoz-technology-website`

## Step 5: Connect Your Custom Domain

### GitHub Settings:
1. In Pages settings, add your custom domain
2. Domain: `your-domain.com` (replace with actual domain)
3. ✅ Enforce HTTPS
4. Save

### Hostinger DNS Configuration:
```
Type: A     | Name: @   | Value: 185.199.108.153
Type: A     | Name: @   | Value: 185.199.109.153  
Type: A     | Name: @   | Value: 185.199.110.153
Type: A     | Name: @   | Value: 185.199.111.153
Type: CNAME | Name: www | Value: codoztech.github.io
```

## 🎯 QUICK START (After Git Installation):

Copy and paste these commands one by one:

```powershell
cd "c:\Users\uk154\Downloads\final-file\skilline-landing-page-main"
git config --global user.name "Codoz Technology"
git config --global user.email "codoztech@gmail.com"
git init
git add .
git commit -m "Initial commit - Codoz Technology Website"
```

**Then create the repository on GitHub.com manually and push:**

```powershell
git remote add origin https://github.com/codoztech/codoz-technology-website.git
git branch -M main
git push -u origin main
```

## ✅ Final Result:
- **GitHub Repository**: https://github.com/codoztech/codoz-technology-website
- **Live Website**: https://codoztech.github.io/codoz-technology-website
- **Custom Domain**: https://your-domain.com (after DNS setup)

**Need help with any step? Let me know!**