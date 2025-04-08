# Step-by-Step Deployment Guide

This guide will help you deploy your personal site to GitHub Pages, which is a free and easy way to host your site.

## Deploying to GitHub Pages

### 1. Create a GitHub Account

If you don't already have a GitHub account, sign up at [github.com](https://github.com/).

### 2. Create a New Repository

1. Click the "+" icon in the top right corner of GitHub and select "New repository"
2. Name your repository (for example, `my-portfolio` or `username.github.io`)
   - For a personal GitHub Pages site, name it `yourusername.github.io` (replace "yourusername" with your actual GitHub username)
   - For a project site, you can use any name you like
3. Make it public
4. Click "Create repository"

### 3. Initialize Git in Your Project (if not already done)

Open your terminal or command prompt, navigate to your project folder, and run:

```bash
git init
git add .
git commit -m "Initial commit"
```

### 4. Connect Your Local Repository to GitHub

```bash
git remote add origin https://github.com/yourusername/your-repository-name.git
git branch -M main
git push -u origin main
```

Replace `yourusername` and `your-repository-name` with your GitHub username and repository name.

### 5. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to the "GitHub Pages" section
4. Under "Source", select the "main" branch
5. Click "Save"
6. Wait a few minutes for your site to be published

### 6. View Your Site

Your site will be available at:
- `https://yourusername.github.io/` (if you used `yourusername.github.io` as your repository name)
- `https://yourusername.github.io/your-repository-name/` (for any other repository name)

### 7. Updating Your Site

Whenever you want to update your site, make your changes locally, then:

```bash
git add .
git commit -m "Update site with [description of changes]"
git push
```

Your changes will be automatically deployed within a few minutes.

## Using a Custom Domain (Optional)

### 1. Purchase a Domain Name

Buy a domain from any domain registrar (GoDaddy, Namecheap, Google Domains, etc.).

### 2. Configure GitHub Pages

1. In your repository, go to "Settings" > "Pages"
2. Under "Custom domain", enter your domain name (e.g., `www.yourdomain.com`)
3. Click "Save"
4. Check "Enforce HTTPS" (only available after DNS propagation is complete)

### 3. Configure DNS with Your Domain Provider

#### For an apex domain (example.com):
Add these A records pointing to GitHub's servers:
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

#### For a www subdomain:
Add a CNAME record pointing `www` to `yourusername.github.io`.

### 4. Wait for DNS Propagation

DNS changes may take 24-48 hours to fully propagate.

## Troubleshooting

- If your site doesn't appear, check the "GitHub Pages" section in repository settings for any error messages
- Make sure your repository is public
- Verify that your HTML file is named `index.html` and is in the root of your repository

## Need More Help?

Refer to the [official GitHub Pages documentation](https://docs.github.com/en/pages) for more detailed information. 