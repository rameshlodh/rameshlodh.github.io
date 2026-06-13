# DevOps Portfolio Site

A personal portfolio site auto-deployed to GitHub Pages using GitHub Actions CI/CD.

## Setup

1. Create a GitHub repo and push this code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/web-hosting.git
   git push -u origin main
   ```

2. Enable GitHub Pages:
   - Go to repo **Settings → Pages**
   - Source: **GitHub Actions**

3. Your site will be live at: `https://YOUR_USERNAME.github.io/web-hosting/`

## How the CI/CD Works

Every push to `main` triggers `.github/workflows/deploy.yml` which:
1. Checks out the code
2. Uploads site files as a Pages artifact
3. Deploys to GitHub Pages

No build step needed — it's pure HTML/CSS served directly.

## Customize

Edit `index.html` to update your info, push to `main`, and it auto-deploys.
