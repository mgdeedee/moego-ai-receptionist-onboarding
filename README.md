# MoeGo AI Onboarding — Live

Single-page onboarding form for MoeGo AI receptionist setup. One form per location (URL param `?location=`). Auto-saves to browser localStorage.

---

## Deploy with Vercel（推荐，最简单）

### 方式 A：连 GitHub（推荐）

1. 把本文件夹推送到 GitHub（若还没推，见下方 GitHub 步骤 1–2）。
2. 打开 [vercel.com](https://vercel.com) → 用 GitHub 登录。
3. **Add New… → Project** → 选你的 `moego-onboarding` 仓库 → **Import**。
4. 不用改设置，直接点 **Deploy**。
5. 几十秒后会给一个链接，例如：`https://moego-onboarding-xxx.vercel.app`。

之后每次 `git push` 都会自动重新部署。

### 方式 B：本地上传（不碰 GitHub）

1. 打开 [vercel.com](https://vercel.com) → 登录。
2. **Add New… → Project** → 选 **Deploy with CLI**。
3. 终端里执行（先装 CLI：`npm i -g vercel`）：

```bash
cd /Users/manchil/moego-onboarding-live
vercel
```

按提示登录、确认项目名，会得到一个 live 链接。

---

## Deploy to GitHub Pages（免费）

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

---

**多 location 链接**（Vercel 或 GitHub Pages 都适用）

- 默认 (Avondale): `/` 或 `/?location=avondale`
- Gilbert: `/?location=gilbert`
- 其他: `/?location=你的slug`

数据按 location 存在浏览器 localStorage，无需后端。
