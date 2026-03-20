# Quick Start: Deploy to GitHub Pages

## 🚀 3 Simple Steps

### Step 1: Copy All Files to Your Repository

Copy all files from this folder to your `karthiksethuram.github.io` repository:

```bash
# Navigate to your GitHub Pages repository
cd /path/to/karthiksethuram.github.io

# Copy all files from the portfolio folder
cp -r /path/to/github-pages-ready/* .
```

Or manually copy these files:
- `index.html` - Main page
- `assets/` - CSS and JavaScript files
- `README.md` - Project documentation

### Step 2: Commit and Push to GitHub

```bash
git add .
git commit -m "Deploy portfolio website"
git push origin main
```

### Step 3: View Your Live Portfolio

Your website will be live at: **https://karthiksethuram.github.io**

It may take 1-5 minutes for GitHub Pages to process and deploy. If you don't see it immediately, try refreshing your browser or clearing the cache.

## ✅ What You Get

✓ Professional portfolio website  
✓ Responsive design (mobile, tablet, desktop)  
✓ Interactive project showcase with filtering  
✓ Complete experience timeline  
✓ Technical skills organized by category  
✓ Education section  
✓ Contact information  

## 📝 Updating Your Portfolio

To add new projects or update content:

1. **Edit the HTML directly** - Open `index.html` and find the projects section
2. **Or use the source code** - Go back to the Manus project and update `client/src/data/portfolio.ts`
3. **Rebuild** - Run `npm run build` in the Manus project
4. **Copy new files** - Replace the `index.html` and `assets/` folder
5. **Push to GitHub** - Commit and push your changes

## 🎨 Customizing Colors

To change the color scheme, edit the CSS in `assets/index-*.css`:

- Deep Slate Blue: `#1e293b` → Change to your preferred primary color
- Vibrant Teal: `#06b6d4` → Change to your preferred accent color

## 🔗 Important Links

- **Your Portfolio**: https://karthiksethuram.github.io
- **GitHub Repository**: https://github.com/karthiksethuram/karthiksethuram.github.io
- **GitHub Pages Help**: https://docs.github.com/en/pages

## ❓ Troubleshooting

**Website not showing?**
- Wait 5-10 minutes for GitHub to process
- Check that your repository is public
- Verify the repository name is `karthiksethuram.github.io`

**Styles look broken?**
- Clear your browser cache (Ctrl+Shift+Delete)
- Try a different browser
- Check the browser console for errors

**Need to make changes?**
- Edit the files directly in the repository
- Or go back to the Manus project and rebuild
- Always commit and push changes to see them live

---

**Congratulations! Your portfolio is now live! 🎉**
