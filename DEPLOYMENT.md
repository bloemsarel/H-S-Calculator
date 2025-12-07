# 🚀 Quick Deployment Guide for GitHub Pages

## Step-by-Step Instructions

### 1️⃣ Create GitHub Repository

1. Go to https://github.com and log in
2. Click the **"+"** button (top right) → **"New repository"**
3. Repository name: `hs-fluid-calculator` (or your preferred name)
4. Description: "Holliday-Segar Fluid Calculator for fluid management - all ages"
5. Select **Public**
6. ✅ **DO NOT** check "Add a README file"
7. Click **"Create repository"**

### 2️⃣ Upload Files

You have two options:

#### Option A: Web Upload (Easiest)
1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop these files:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Commit message: "Initial commit: Holliday-Segar Calculator"
4. Click **"Commit changes"**

#### Option B: Git Command Line
```bash
# Initialize git in your project folder
cd /path/to/your/files
git init

# Add all files
git add index.html README.md LICENSE .gitignore

# Commit
git commit -m "Initial commit: Holliday-Segar Calculator"

# Connect to GitHub
git remote add origin https://github.com/[YOUR-USERNAME]/hs-fluid-calculator.git
git branch -M main

# Push to GitHub
git push -u origin main
```

### 3️⃣ Enable GitHub Pages

1. In your repository, click **"Settings"** (top menu)
2. Click **"Pages"** in the left sidebar
3. Under **"Source"**:
   - Select **"Deploy from a branch"**
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 1-2 minutes for deployment

### 4️⃣ Access Your Calculator

Your calculator will be live at:
```
https://[YOUR-USERNAME].github.io/hs-fluid-calculator/
```

**Example:** If your username is `bloemsarel`, the URL would be:
```
https://bloemsarel.github.io/hs-fluid-calculator/
```

### 5️⃣ Test on Mobile

1. Open the URL on your smartphone
2. Test the calculator with different weights
3. Try selecting different diagnoses
4. Verify the layout looks good

### 6️⃣ Add to Home Screen (Optional)

#### iPhone/iPad:
1. Open in Safari
2. Tap share button (□↑)
3. Scroll → "Add to Home Screen"
4. Name it "HS Calculator"
5. Tap "Add"

#### Android:
1. Open in Chrome
2. Tap ⋮ (three dots)
3. "Add to Home screen"
4. Name it and tap "Add"

## 🔄 Making Updates

### To update the calculator later:

1. Go to your repository on GitHub
2. Click on the file you want to edit (e.g., `index.html`)
3. Click the ✏️ (pencil) icon to edit
4. Make your changes
5. Scroll down, add commit message
6. Click **"Commit changes"**
7. Changes will be live in 1-2 minutes

## ⚠️ Troubleshooting

### Calculator doesn't load:
- Wait 2-3 minutes after enabling GitHub Pages
- Check that your repository is **public**
- Verify the URL is correct: `https://[username].github.io/[repo-name]/`
- Clear browser cache and try again

### Layout looks broken on mobile:
- Make sure you uploaded the complete `index.html` file
- Check that the viewport meta tag is present
- Test in different browsers (Chrome, Safari, Firefox)

### Getting 404 error:
- Verify GitHub Pages is enabled in Settings → Pages
- Check that `index.html` is in the root folder
- Make sure the repository is public

## 📱 Share Your Calculator

Once deployed, share the link with:
- Colleagues via email or messaging apps
- Department group chats
- Hospital intranet (if allowed)
- Medical education platforms

## 🎯 Custom Domain (Advanced)

Want a custom URL like `calculator.yourdomain.com`?

1. Buy a domain from a registrar
2. In repository Settings → Pages → Custom domain
3. Enter your domain
4. Add DNS records at your registrar:
   ```
   Type: CNAME
   Host: calculator (or www)
   Value: [your-username].github.io
   ```
5. Wait for DNS propagation (can take 24 hours)

## 📊 Analytics (Optional)

To track usage:

1. Get a Google Analytics ID
2. Edit `index.html`
3. Add before `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## ✅ Checklist

- [ ] Created GitHub repository
- [ ] Uploaded all files (index.html, README.md, LICENSE, .gitignore)
- [ ] Enabled GitHub Pages in Settings
- [ ] Tested calculator URL in browser
- [ ] Verified mobile responsiveness
- [ ] Added to mobile home screen
- [ ] Shared with colleagues

## 🆘 Need Help?

- Check GitHub Pages documentation: https://pages.github.com/
- GitHub community forum: https://github.community/
- Open an issue in your repository

---

**Congratulations! Your calculator is now live! 🎉**

Share it, use it, and help improve patient care!
