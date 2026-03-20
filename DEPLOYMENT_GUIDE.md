# Deployment Guide: Portfolio Website to GitHub Pages

This guide provides step-by-step instructions for deploying your portfolio website to GitHub Pages.

## Prerequisites

- Git installed on your machine
- GitHub account with the repository `karthiksethuram.github.io` already created
- Node.js and npm installed locally

## Step 1: Build the Website

Before deploying, you need to build the production-ready version of the website:

```bash
cd /home/ubuntu/portfolio-website
npm run build
```

This command will create a `dist` folder containing all the optimized files ready for deployment.

## Step 2: Clone Your GitHub Repository

If you haven't already cloned your repository locally, do so now:

```bash
git clone https://github.com/karthiksethuram/karthiksethuram.github.io.git
cd karthiksethuram.github.io
```

## Step 3: Copy Build Files to Repository

Copy all files from the `dist` folder to your repository root:

```bash
# From your portfolio-website directory
cp -r dist/* /path/to/karthiksethuram.github.io/
```

## Step 4: Commit and Push to GitHub

Navigate to your repository and commit the changes:

```bash
cd /path/to/karthiksethuram.github.io
git add .
git commit -m "Deploy portfolio website"
git push origin main
```

## Step 5: Verify Deployment

Your website should now be live at: `https://karthiksethuram.github.io`

It may take a few minutes for GitHub Pages to process and deploy your site. If you don't see it immediately, try refreshing your browser or clearing the cache.

## Step 6: Configure GitHub Pages Settings (if needed)

1. Go to your repository on GitHub
2. Click on "Settings"
3. Scroll to "GitHub Pages" section
4. Ensure "Source" is set to "main branch" or "main branch /root directory"
5. Save settings

## Updating Your Portfolio

To add new projects or update content in the future:

1. **Edit the portfolio data** in `/client/src/data/portfolio.ts`
2. **Add new project images** if needed (upload via `manus-upload-file --webdev`)
3. **Rebuild the website**: `npm run build`
4. **Copy updated files** to your GitHub repository
5. **Commit and push** the changes

## File Structure After Build

The `dist` folder will contain:

```
dist/
├── index.html          (Main HTML file)
├── assets/             (CSS, JS, and other assets)
└── ...
```

All these files should be copied to your GitHub Pages repository.

## Troubleshooting

### Website not showing up after push
- Wait 5-10 minutes for GitHub Pages to process
- Check that you're accessing the correct URL
- Verify that your repository is set to public

### Styles not loading
- Clear your browser cache (Ctrl+Shift+Delete or Cmd+Shift+Delete)
- Check the browser console for any 404 errors
- Ensure all asset paths are correct in the built files

### Images not displaying
- Verify that image URLs are correct in the code
- Check that external CDN links are accessible
- Ensure image files were properly copied to the repository

## Custom Domain (Optional)

If you want to use a custom domain instead of `karthiksethuram.github.io`:

1. Add a `CNAME` file to your repository root with your domain name
2. Configure DNS settings with your domain provider
3. Update GitHub Pages settings to use your custom domain

## Next Steps

After deployment, consider:

1. **Adding more projects** - Update the projects array in `portfolio.ts`
2. **Implementing dark mode** - Uncomment the `switchable` prop in `App.tsx`
3. **Adding a blog section** - Create a new page for technical articles
4. **Setting up analytics** - Track visitor engagement
5. **Optimizing performance** - Monitor and improve page load times

## Support

For issues or questions about deployment, refer to the [GitHub Pages documentation](https://docs.github.com/en/pages).
