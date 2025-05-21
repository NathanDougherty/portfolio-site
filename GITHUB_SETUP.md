# GitHub Repository Setup Guide

Follow these steps to push your portfolio site to GitHub and configure it for deployment with GitHub Pages or Vercel.

## 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository `portfolio`
4. Set it to "Public"
5. Do not initialize it with a README, .gitignore, or license
6. Click "Create repository"

## 2. Initialize Git and Push Your Code

Run these commands in your terminal from the `portfolio-site` directory:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial portfolio website commit"

# Add remote GitHub repository (replace USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push to GitHub
git push -u origin main
```

## 3. Deploy with Vercel (Recommended)

1. Go to [Vercel](https://vercel.com) and sign up/in with your GitHub account
2. Click "New Project"
3. Import your GitHub repository
4. Keep the default settings and click "Deploy"
5. Your site will be deployed to a URL like: `https://portfolio-yourusername.vercel.app`
6. You can set up a custom domain in Vercel dashboard later

## 4. Alternative: Deploy with GitHub Pages

If you're using GitHub Pages instead of Vercel:

1. Go to your GitHub repository
2. Go to "Settings" > "Pages"
3. Under "Source", select "GitHub Actions"
4. Your site will be deployed automatically using the workflow in `.github/workflows/deploy.yml`
5. Your site will be available at `https://YOUR_USERNAME.github.io/portfolio`

## Updating Your Site

To update your site after making changes:

```bash
# Add all changed files
git add .

# Commit changes
git commit -m "Update portfolio content"

# Push to GitHub
git push
```

Your site will automatically be rebuilt and deployed. 