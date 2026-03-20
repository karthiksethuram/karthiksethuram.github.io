# Complete GitHub Pages Setup Guide

## Prerequisites

- GitHub account (you already have this)
- Repository named `karthiksethuram.github.io` (you already have this)
- Git installed on your computer

## Option 1: Using Git Command Line (Recommended)

### Step 1: Clone Your Repository

```bash
git clone https://github.com/karthiksethuram/karthiksethuram.github.io.git
cd karthiksethuram.github.io
```

### Step 2: Clear Existing Files (if any)

```bash
# Remove all existing files except .git
git rm -r . --cached
rm -r * .gitignore .github
```

### Step 3: Copy Portfolio Files

Copy all files from the `github-pages-ready` folder to your repository:

```bash
# Copy from wherever you downloaded the files
cp -r /path/to/github-pages-ready/* .
```

Your repository should now contain:
- `index.html`
- `assets/` (folder)
- `README.md`
- `QUICK_START.md`
- `DEPLOYMENT_GUIDE.md`
- `.gitignore`

### Step 4: Commit and Push

```bash
git add .
git commit -m "Initial portfolio website deployment"
git push origin main
```

### Step 5: Verify Deployment

Wait 1-5 minutes, then visit: **https://karthiksethuram.github.io**

---

## Option 2: Using GitHub Web Interface

### Step 1: Go to Your Repository

1. Open https://github.com/karthiksethuram/karthiksethuram.github.io
2. Click the green "Code" button
3. Click "Upload files"

### Step 2: Upload Files

1. Drag and drop all files from `github-pages-ready/` folder
2. Or click "choose your files" and select them one by one

### Step 3: Commit Changes

1. Add commit message: "Initial portfolio website deployment"
2. Click "Commit changes"

### Step 4: Verify Deployment

Wait 1-5 minutes, then visit: **https://karthiksethuram.github.io**

---

## Option 3: Using GitHub Desktop (Easiest for Beginners)

### Step 1: Install GitHub Desktop

Download from: https://desktop.github.com/

### Step 2: Clone Your Repository

1. Open GitHub Desktop
2. Click "File" → "Clone Repository"
3. Select `karthiksethuram/karthiksethuram.github.io`
4. Choose a local folder

### Step 3: Copy Files

1. Open the cloned folder on your computer
2. Copy all files from `github-pages-ready/` into this folder
3. Replace any existing files

### Step 4: Commit and Push

1. GitHub Desktop will show all changed files
2. Add commit message: "Initial portfolio website deployment"
3. Click "Commit to main"
4. Click "Push origin"

### Step 5: Verify Deployment

Wait 1-5 minutes, then visit: **https://karthiksethuram.github.io**

---

## File Structure

After uploading, your repository should look like this:

```
karthiksethuram.github.io/
├── index.html              ← Main portfolio page
├── README.md               ← Project documentation
├── QUICK_START.md          ← Quick reference
├── DEPLOYMENT_GUIDE.md     ← Detailed deployment info
├── GITHUB_SETUP.md         ← This file
├── .gitignore              ← Git ignore rules
└── assets/
    ├── index-BZE5YYmE.css  ← Styles
    └── index-BB697Hzl.js   ← JavaScript
```

---

## Verify Your Setup

### Check if GitHub Pages is Enabled

1. Go to https://github.com/karthiksethuram/karthiksethuram.github.io/settings
2. Scroll to "GitHub Pages" section
3. Verify "Source" is set to "Deploy from a branch"
4. Verify "Branch" is set to "main" and "/ (root)"

### Check Deployment Status

1. Go to your repository
2. Click "Deployments" tab
3. Look for the latest deployment
4. Status should be "Active"

---

## Troubleshooting

### Website Shows 404 Error

**Problem**: Page not found  
**Solution**:
- Wait 5-10 minutes for GitHub to process
- Check repository name is exactly `karthiksethuram.github.io`
- Verify `index.html` is in the root directory
- Clear browser cache and try again

### Website Shows Blank Page

**Problem**: Page loads but shows nothing  
**Solution**:
- Check browser console for errors (F12)
- Verify all files in `assets/` folder are present
- Try a different browser
- Clear browser cache

### Styles Look Broken

**Problem**: Website shows but colors/layout are wrong  
**Solution**:
- Clear browser cache (Ctrl+Shift+Delete)
- Check that `assets/` folder exists with CSS file
- Verify file permissions are correct
- Try accessing from incognito/private window

### Changes Not Showing

**Problem**: Made changes but website doesn't update  
**Solution**:
- Wait 5 minutes for GitHub to rebuild
- Clear browser cache completely
- Check that you pushed the changes to GitHub
- Verify the deployment completed successfully

---

## Making Updates

### To Update Your Portfolio

1. Edit `index.html` directly in GitHub web interface, or
2. Go back to the Manus project and update `client/src/data/portfolio.ts`
3. Rebuild with `npm run build`
4. Copy new `index.html` and `assets/` files to your repository
5. Commit and push changes

### To Add New Projects

Edit the HTML file and find the "Featured Projects" section, then add a new project card following the same format.

---

## Custom Domain (Optional)

If you want to use a custom domain like `karthikeyan.com`:

1. Purchase a domain from a registrar (GoDaddy, Namecheap, etc.)
2. Go to your repository Settings → Pages
3. Under "Custom domain", enter your domain name
4. Follow the DNS configuration instructions from your domain registrar
5. GitHub will automatically handle the SSL certificate

---

## Support

For more help:
- GitHub Pages Documentation: https://docs.github.com/en/pages
- GitHub Community: https://github.community
- Contact me: ksethuramam1992@gmail.com

---

**You're all set! Your portfolio is now live on GitHub Pages! 🎉**
