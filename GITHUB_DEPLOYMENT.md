# GitHub Deployment Guide

## 🚀 Publishing Your Portfolio to GitHub Pages

This guide will help you deploy your beautiful glassmorphism portfolio to GitHub Pages for free!

## 📋 Prerequisites

- ✅ GitHub account (you have one: github.com/nishanta09)
- ✅ Git installed on your computer
- ✅ Your portfolio files are ready

## 🎯 Step-by-Step Deployment

### Step 1: Initialize Git Repository

1. **Open Command Prompt/PowerShell**
2. **Navigate to your portfolio folder**:
   ```bash
   cd "C:\Users\nisha\OneDrive\projects\html and css\portfolio"
   ```

3. **Initialize Git**:
   ```bash
   git init
   ```

4. **Add all files**:
   ```bash
   git add .
   ```

5. **Make first commit**:
   ```bash
   git commit -m "Initial commit: Glassmorphism portfolio with orbital skills design"
   ```

### Step 2: Create GitHub Repository

1. **Go to GitHub**: [github.com](https://github.com)
2. **Click "+" → "New repository"**
3. **Repository settings**:
   - **Repository name**: `portfolio` (or `nishant-portfolio`)
   - **Description**: `Software Developer Portfolio - Glassmorphism Design`
   - **Visibility**: Public (required for GitHub Pages)
   - **Don't initialize** with README, .gitignore, or license

4. **Click "Create repository"**

### Step 3: Connect Local to GitHub

1. **Copy the repository URL** from GitHub (Quick setup section)
2. **Add remote origin** (replace with your actual URL):
   ```bash
   git remote add origin https://github.com/nishanta09/portfolio.git
   ```

3. **Push to GitHub**:
   ```bash
   git branch -M main
   git push -u origin main
   ```

### Step 4: Enable GitHub Pages

1. **Go to your repository on GitHub**
2. **Click "Settings" tab**
3. **Find "Pages" in left menu**
4. **Source settings**:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
   - **Click "Save"**

5. **Wait a few minutes** for deployment

### Step 5: Get Your Portfolio URL

1. **Go back to Settings → Pages**
2. **Your portfolio URL will be displayed**:
   ```
   https://nishanta09.github.io/portfolio/
   ```

## 🎨 Alternative: GitHub Pages with Custom Domain

### Option 1: Repository Name Method
If you name your repository `nishanta09.github.io`, your site will be available at:
```
https://nishanta09.github.io/
```

### Option 2: Custom Domain
1. **Buy a domain** (optional)
2. **Add CNAME file** in portfolio folder:
   ```
   yourdomain.com
   ```
3. **Configure DNS** settings with your domain provider

## 🔧 Common Issues & Solutions

### Issue 1: "Page not found"
**Solution**: Wait 5-10 minutes after enabling Pages

### Issue 2: "404 error"
**Solution**: 
- Check your repository name
- Ensure main branch is selected
- Verify files are in root folder

### Issue 3: "Styles not loading"
**Solution**: 
- Check CSS file paths in HTML
- Ensure files are pushed to GitHub
- Clear browser cache

### Issue 4: "Form not working"
**Solution**: 
- GitHub Pages doesn't support server-side forms
- Your Formspree setup should work fine
- Test the form after deployment

## 📱 Testing Your Live Portfolio

1. **Visit your URL**: `https://nishanta09.github.io/portfolio/`
2. **Test all sections**:
   - Navigation scrolling
   - Contact form submission
   - Social links
   - Responsive design
   - Animations

## 🚀 Advanced Deployment Options

### Option 1: GitHub Actions (Automatic)
Create `.github/workflows/deploy.yml`:
```yaml
name: Deploy to GitHub Pages
on:
  push:
    branches: [ main ]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./
```

### Option 2: Manual Deployment Script
Create `deploy.bat`:
```batch
@echo off
echo Deploying to GitHub...
git add .
git commit -m "Update portfolio"
git push origin main
echo Deployment complete!
pause
```

## 🎯 Pro Tips for Your Portfolio

### 1. Optimize for Performance
- Compress images before adding
- Minimize CSS/JS files
- Enable gzip compression

### 2. SEO Optimization
- Update meta tags in HTML
- Add sitemap.xml
- Submit to Google Search Console

### 3. Analytics
- Add Google Analytics
- Track visitor statistics
- Monitor form submissions

### 4. Backup Strategy
- Keep local copy
- Use GitHub branches for features
- Tag releases

## 📞 What to Include in Your README

Update your README.md with:
```markdown
# Nishant Kumar - Software Developer Portfolio

## 🌐 Live Demo
[https://nishanta09.github.io/portfolio/](https://nishanta09.github.io/portfolio/)

## 🛠️ Technologies Used
- HTML5, CSS3, JavaScript
- Glassmorphism Design
- Formspree for contact form
- Font Awesome Icons

## 📱 Features
- Responsive Design
- Orbital Skills Section
- Contact Form
- Social Links

## 🚀 Getting Started
1. Clone this repository
2. Open `portfolio.html` in browser
3. Or deploy to your own GitHub Pages

## 📧 Contact
- Email: nishantsng.dev9@gmail.com
- LinkedIn: [linkedin.com/in/nishant-kumar-66037a187](https://www.linkedin.com/in/nishant-kumar-66037a187)
- GitHub: [github.com/nishanta09](https://github.com/nishanta09)
```

## 🎉 Deployment Checklist

- [ ] Git repository initialized
- [ ] Files committed to Git
- [ ] GitHub repository created
- [ ] Code pushed to GitHub
- [ ] GitHub Pages enabled
- [ ] Custom domain (optional)
- [ ] Contact form tested
- [ ] Social links verified
- [ ] Mobile responsiveness checked
- [ ] All animations working

## 🔗 Useful Links

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Status](https://www.githubstatus.com/)
- [Custom Domain Guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

---

## 🎯 Quick Commands Summary

```bash
# Navigate to portfolio folder
cd "C:\Users\nisha\OneDrive\projects\html and css\portfolio"

# Initialize Git
git init
git add .
git commit -m "Initial portfolio commit"

# Add GitHub remote
git remote add origin https://github.com/nishanta09/portfolio.git
git branch -M main

# Push to GitHub
git push -u origin main

# Future updates
git add .
git commit -m "Update portfolio content"
git push origin main
```

## 🚀 Ready to Launch!

Once you complete these steps, your portfolio will be live at:
**https://nishanta09.github.io/portfolio/**

Your beautiful glassmorphism portfolio with orbital skills design will be accessible to employers and clients worldwide!

*Deployment time: ~10 minutes*
