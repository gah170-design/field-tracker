# 🌾 Field Tracker — Deployment Guide

## Files in this folder
```
index.html      ← Main app
manifest.json   ← Makes it installable as a PWA
sw.js           ← Service worker (offline support)
icon-192.png    ← Home screen icon
icon-512.png    ← Home screen icon (large)
```

---

## Deploy to GitHub Pages (free, HTTPS, ~5 minutes)

### 1. Create a GitHub account
Go to https://github.com and sign up if you don't have one.

### 2. Create a new repository
- Click the **+** in the top right → **New repository**
- Name it anything, e.g. `field-tracker`
- Set it to **Public**
- Click **Create repository**

### 3. Upload the files
- On your new repo page, click **uploading an existing file**
- Drag all 5 files from this folder into the upload area
- Click **Commit changes**

### 4. Enable GitHub Pages
- Go to your repo **Settings** → **Pages** (left sidebar)
- Under **Source**, select **Deploy from a branch**
- Branch: `main` / Folder: `/ (root)`
- Click **Save**

### 5. Wait ~60 seconds, then visit your app
Your URL will be:
```
https://YOUR-USERNAME.github.io/field-tracker/
```

---

## Install on iPhone (Safari)
1. Open the URL in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add**
5. The app will appear on your home screen and open full-screen

## Install on Android (Chrome)
1. Open the URL in **Chrome**
2. Tap the **⋮** menu → **Add to Home screen**
3. Tap **Add**

---

## Notes
- **GPS requires HTTPS** — GitHub Pages provides this automatically ✓
- **Offline support** — once visited, the app and any satellite tiles
  you've panned over will be cached for use in areas with no signal
- **Data is stored locally** on the phone in localStorage — it persists
  between sessions but stays on that device
- **No account, no server, no cost** — GitHub Pages is completely free
  for public repos
