# MoeGo AI Onboarding — Live

Single-page onboarding form for MoeGo AI receptionist setup. One form per location (URL param `?location=`). Auto-saves to browser localStorage.

## Deploy to GitHub Pages (free, live in ~2 min)

### 1. Create a new repo on GitHub

- Go to [github.com/new](https://github.com/new)
- Repository name: e.g. `moego-onboarding` (or any name)
- Public, no need to add README (this folder already has files)
- Create repository

### 2. Push this folder to the repo

In terminal, from this folder (`moego-onboarding-live`):

```bash
cd /Users/manchil/moego-onboarding-live
git init
git add index.html README.md
git commit -m "MoeGo onboarding live"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/moego-onboarding.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username and `moego-onboarding` with your repo name.

### 3. Turn on GitHub Pages

- Open the repo on GitHub → **Settings** → **Pages**
- Under **Source**: choose **Deploy from a branch**
- Branch: **main**, Folder: **/ (root)** → Save
- Wait 1–2 minutes. Your site will be at:

**https://YOUR_USERNAME.github.io/moego-onboarding/**

### URLs by location

- Default (Avondale): `https://YOUR_USERNAME.github.io/moego-onboarding/`
- Gilbert: `https://YOUR_USERNAME.github.io/moego-onboarding/?location=gilbert`
- Any other location: `?location=your-location-slug`

Data is saved per location in the browser (localStorage). No backend required.
