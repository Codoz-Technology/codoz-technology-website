# 🚀 Complete Deployment Guide: GitHub + Hostinger Domain

## Step 1: Install Git (Required)

### Option A: Download Git for Windows
1. Go to: https://git-scm.com/download/win
2. Download and install Git for Windows
3. During installation, select "Git from the command line and also from 3rd-party software"
4. Restart your computer after installation

### Option B: Install via GitHub Desktop (Easier)
1. Go to: https://desktop.github.com/
2. Download and install GitHub Desktop
3. Sign in with your GitHub account
4. Use the GUI interface (no command line needed)

## Step 2: Create GitHub Repository

### Method A: Using GitHub Website (Recommended)
1. Go to https://github.com
2. Sign in or create account
3. Click "+" → "New repository"
4. Repository name: `codoz-technology-website`
5. Description: "Official website for Codoz Technology - Digital Solutions"
6. Set as Public
7. ✅ Add README file
8. ✅ Add .gitignore (select "Node" template)
9. Click "Create repository"

### Method B: Using GitHub Desktop
1. Open GitHub Desktop
2. File → New Repository
3. Name: `codoz-technology-website`
4. Local path: Select your project folder
5. Click "Create Repository"

## Step 3: Upload Your Files

### Using GitHub Desktop (Easiest):
1. File → Add Local Repository
2. Select your project folder: `c:\Users\uk154\Downloads\final-file\skilline-landing-page-main`
3. All files will appear in "Changes" tab
4. Write commit message: "Initial website launch - Codoz Technology"
5. Click "Commit to main"
6. Click "Publish repository" (top right)

### Using GitHub Website (Alternative):
1. In your new repository, click "uploading an existing file"
2. Drag and drop all files from your project folder
3. Write commit message: "Initial website launch"
4. Click "Commit changes"

## Step 4: Enable GitHub Pages

1. In your GitHub repository, go to **Settings** tab
2. Scroll down to **Pages** section (left sidebar)
3. Source: Select "Deploy from a branch"
4. Branch: Select "main" 
5. Folder: Select "/ (root)"
6. Click **Save**
7. Your site will be available at: `https://YOUR_USERNAME.github.io/codoz-technology-website`

## Step 5: Connect Custom Domain (Hostinger)

### A. Configure GitHub Pages:
1. In GitHub Pages settings (Step 4)
2. Custom domain: Enter your domain (e.g., `codoztech.com`)
3. ✅ Enforce HTTPS
4. Click Save

### B. Configure Hostinger DNS:
1. Login to Hostinger control panel
2. Go to **DNS Zone Editor**
3. Add these records:

**For root domain (codoztech.com):**
```
Type: A
Name: @
Value: 185.199.108.153
TTL: 14400

Type: A  
Name: @
Value: 185.199.109.153
TTL: 14400

Type: A
Name: @
Value: 185.199.110.153
TTL: 14400

Type: A
Name: @
Value: 185.199.111.153
TTL: 14400
```

**For www subdomain:**
```
Type: CNAME
Name: www
Value: YOUR_USERNAME.github.io
TTL: 14400
```

### C. Create CNAME file in GitHub:
1. In your repository, create new file called `CNAME`
2. Content: Just your domain name: `codoztech.com`
3. Commit the file

## Step 6: Verify Deployment (Wait 24-48 hours)

1. **GitHub Pages URL**: `https://YOUR_USERNAME.github.io/codoz-technology-website`
2. **Custom Domain**: `https://codoztech.com` (after DNS propagation)
3. **Check DNS**: Use https://whatsmydns.net to verify DNS propagation

## 🎯 Quick Commands (After Git Installation):

```bash
# Navigate to your project
cd "c:\Users\uk154\Downloads\final-file\skilline-landing-page-main"

# Initialize git
git init

# Add all files
git add .

# Commit files
git commit -m "Initial website launch - Codoz Technology"

# Add remote repository (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/codoz-technology-website.git

# Push to GitHub
git push -u origin main
```

## 🔧 Troubleshooting:

**Issue**: DNS not working
**Solution**: Wait 24-48 hours for DNS propagation, check Hostinger DNS settings

**Issue**: GitHub Pages not building
**Solution**: Check repository settings, ensure index.html is in root folder

**Issue**: Images not loading
**Solution**: Check file paths are relative (img/filename.jpg not /img/filename.jpg)

## 📞 Need Help?

If you encounter any issues:
1. Check GitHub repository settings
2. Verify DNS settings in Hostinger
3. Test with GitHub Pages URL first
4. Contact me for additional support

**Your website will be live at your custom domain within 24-48 hours!**