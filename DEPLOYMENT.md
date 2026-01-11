# 🚀 Deployment Guide

## Quick Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon (top right) → "New repository"
3. Repository name: `chef-shaker-portfolio` (or your choice)
4. Description: "Professional culinary portfolio - 23+ years of excellence"
5. Make it **Public**
6. DO NOT initialize with README (we already have one)
7. Click "Create repository"

### Step 2: Upload Files to GitHub

**Option A: Using GitHub Web Interface (Easiest)**

1. On your new repository page, click "uploading an existing file"
2. Drag and drop ALL files from your website folder:
   - index.html
   - README.md
   - .gitignore
   - css/ (folder)
   - js/ (folder)
   - images/ (folder)
3. Write commit message: "Initial commit - Chef Shaker Portfolio"
4. Click "Commit changes"

**Option B: Using Git Command Line**

```bash
# Navigate to your website folder
cd chef-shaker-portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit - Chef Shaker Portfolio"

# Connect to GitHub (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/chef-shaker-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source":
   - Branch: Select `main`
   - Folder: Select `/ (root)`
5. Click "Save"
6. Wait 1-2 minutes

Your site will be live at:
```
https://YOUR-USERNAME.github.io/chef-shaker-portfolio/
```

### Step 4: Custom Domain (Optional)

If you want your own domain (e.g., chefshaker.com):

1. Buy a domain from any registrar (Namecheap, GoDaddy, etc.)
2. In your repository Settings → Pages:
   - Enter your custom domain
   - Click "Save"
3. In your domain registrar's DNS settings, add:
   - Type: `A` Record
   - Host: `@`
   - Points to:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Type: `CNAME` Record
   - Host: `www`
   - Points to: `YOUR-USERNAME.github.io`

Wait 24-48 hours for DNS propagation.

---

## Alternative Deployments

### Deploy to Netlify (Free & Fast)

1. Go to [Netlify](https://www.netlify.com) and sign up
2. Drag and drop your website folder onto Netlify
3. Done! Your site is live instantly
4. Netlify provides:
   - Free SSL certificate
   - Custom domain support
   - Automatic deploys from GitHub

### Deploy to Vercel (Free & Fast)

1. Go to [Vercel](https://vercel.com) and sign up with GitHub
2. Click "Import Project"
3. Select your GitHub repository
4. Click "Deploy"
5. Done! Your site is live

---

## Updating Your Website

### When you want to make changes:

**Using GitHub Web:**
1. Go to your repository
2. Navigate to the file you want to edit
3. Click the pencil icon (Edit)
4. Make changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for changes to appear on your live site

**Using Git Command Line:**
```bash
# Make your changes to the files
# Then:
git add .
git commit -m "Updated portfolio content"
git push
```

---

## Troubleshooting

**Site not loading?**
- Wait 2-3 minutes after enabling GitHub Pages
- Check that index.html is in the root directory
- Clear your browser cache

**Images not showing?**
- Check image paths in index.html are correct
- Ensure images are in the `images/` folder
- Image filenames are case-sensitive

**CSS/JS not working?**
- Check file paths in index.html
- Ensure css/style.css and js/script.js exist
- Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)

---

## Support

For questions or issues:
- Email: Shakerghamry@yahoo.com
- Check README.md for detailed documentation

**Congratulations! Your portfolio is now live! 🎉**
