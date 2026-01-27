# Dot Journal Website

This folder contains the static website for Dot Journal's Terms of Service and Privacy Policy, required by Apple App Store guidelines.

## Deployment to GitHub Pages

### Option 1: Using GitHub Actions (Recommended)

1. Push this `docs-website` folder to your GitHub repository
2. Go to your repository Settings → Pages
3. Under "Build and deployment":
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/docs-website`
4. Click Save

Your site will be live at: `https://YOUR-USERNAME.github.io/dot-journal/`

### Option 2: Manual Deployment

If your repo is private or you want a custom domain:

1. Create a new branch called `gh-pages`
2. Copy the contents of `docs-website` to the root of that branch
3. Push to GitHub
4. Enable GitHub Pages in Settings → Pages
5. Select `gh-pages` branch

## URLs for App Store Connect

Once deployed, use these URLs in App Store Connect:

- **Privacy Policy URL**: `https://YOUR-USERNAME.github.io/dot-journal/privacy.html`
- **Terms of Service (EULA)**: `https://YOUR-USERNAME.github.io/dot-journal/terms.html`

## Alternative Hosting Options

If you prefer not to use GitHub Pages:

1. **Netlify**: Drag and drop this folder to [Netlify Drop](https://app.netlify.com/drop)
2. **Vercel**: Deploy with `vercel deploy docs-website`
3. **Cloudflare Pages**: Connect your GitHub repo and set build directory to `docs-website`

## Files

- `index.html` - Landing page
- `privacy.html` - Privacy Policy (required by Apple)
- `terms.html` - Terms of Service / EULA (required by Apple)

## Updating Content

To update the Privacy Policy or Terms:

1. Edit `privacy.html` or `terms.html`
2. Update the "Last Updated" date
3. Commit and push changes
4. GitHub Pages will automatically redeploy
