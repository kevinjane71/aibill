# Setup Guide for AIBill GitHub Pages

## 🚀 Quick Setup (5 minutes)

### Step 1: Create New GitHub Repository

1. Go to: **https://github.com/new**

2. Fill in:
   - **Repository name:** `aibill`
   - **Description:** AIBill - Track Your AI Subscriptions (Website)
   - **Visibility:** Public ✅ (required for free GitHub Pages)
   - **DO NOT** check "Add a README file" (we already have files)
   - **DO NOT** add .gitignore or license yet

3. Click **"Create repository"**

---

### Step 2: Push This Folder to GitHub

Open Terminal and run:

```bash
cd /Users/vivek/code/sub-tracker/aibill

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - AIBill website for App Store"

# Add your GitHub repo (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/aibill.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Replace YOUR-USERNAME** with `kevinjane71` (your GitHub username)

---

### Step 3: Enable GitHub Pages

1. Go to your new repository on GitHub:
   `https://github.com/YOUR-USERNAME/aibill`

2. Click **"Settings"** (top menu)

3. Click **"Pages"** (left sidebar under "Code and automation")

4. Under "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** main
   - **Folder:** / (root) ← **Select root, not /docs**
   - Click **"Save"**

5. Wait 2-3 minutes for GitHub to build your site

---

### Step 4: Your Live URLs

After deployment, your pages will be live at:

```
https://kevinjane71.github.io/aibill/
https://kevinjane71.github.io/aibill/privacy.html
https://kevinjane71.github.io/aibill/support.html
```

**Test them!** Click each URL to make sure they work.

---

## 📱 Use in App Store Connect

When submitting your app to Apple, use these URLs:

**Privacy Policy URL:**
```
https://kevinjane71.github.io/aibill/privacy.html
```

**Support URL:**
```
https://kevinjane71.github.io/aibill/support.html
```

**Marketing URL (Optional):**
```
https://kevinjane71.github.io/aibill/
```

---

## ✅ Checklist

- [ ] Create new GitHub repository named `aibill`
- [ ] Run git commands to push files
- [ ] Enable GitHub Pages in Settings → Pages
- [ ] Wait 2-3 minutes
- [ ] Test all URLs in browser
- [ ] Copy URLs to App Store Connect
- [ ] You're done! 🎉

---

## 🔧 Troubleshooting

### Authentication Error When Pushing?

If you get an authentication error:

```bash
# Use personal access token instead
# Go to: https://github.com/settings/tokens
# Create new token with "repo" permissions
# Use token as password when prompted
```

Or use SSH:
```bash
git remote set-url origin git@github.com:kevinjane71/aibill.git
git push -u origin main
```

### "Page Not Found" Error?

- Wait a few more minutes (can take up to 10 minutes)
- Make sure repository is **Public**
- Check that GitHub Pages is enabled in Settings
- Verify files are in the root of the repository

---

## 🎉 You're Done!

Once your pages are live, you can submit your app to the App Store with confidence!
