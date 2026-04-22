<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6c8fff&height=200&section=header&text=DevLog&fontSize=80&fontAlignY=35&desc=Daily%20Work%20Tracker%20for%20Developers&descAlignY=55&descSize=20&fontColor=ffffff&animation=fadeIn" width="100%"/>

<br/>

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Open%20App-6c8fff?style=for-the-badge&logoColor=white)](https://dipak491.github.io/DevLog_daily_tracker/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222?style=for-the-badge&logo=github&logoColor=white)](https://dipak491.github.io/DevLog_daily_tracker/)
[![Mobile Ready](https://img.shields.io/badge/📱%20Mobile-Friendly-3ecf8e?style=for-the-badge)](https://dipak491.github.io/DevLog_daily_tracker/)
[![Themes](https://img.shields.io/badge/🎨%20Themes-5%20Options-a78bfa?style=for-the-badge)](https://dipak491.github.io/DevLog_daily_tracker/)
[![License](https://img.shields.io/badge/License-MIT-f59e0b?style=for-the-badge)](LICENSE)

<br/>

> **A beautiful, secure, cross-device daily work tracker built for developers.**
> Log what you did · what you need to do · what you learned · where you want to improve
> Synced across all devices via GitHub Gist · Protected by password · Works on mobile

<br/>

</div>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 📋 Four Tracking Sections
- ✅ **What I Did** — log completed work with tags (feature, bug, review, meeting)
- 📌 **To-Do** — tasks with priority levels (high / medium / low)
- 📚 **What I Learned** — capture concepts, tricks, tools learned today
- 📈 **Areas to Improve** — track growth areas with urgency levels

</td>
<td width="50%">

### 📱 Fully Mobile Responsive
- Bottom navigation bar for easy thumb access
- Slide-up modals — native mobile feel
- Touch-friendly buttons (44px+ targets)
- Compact date bar and mobile topbar
- Works perfectly on any screen size

</td>
</tr>
<tr>
<td width="50%">

### 🎨 5 Beautiful Themes
- 🌑 **Dark** — deep dark (default)
- ☀️ **Light** — clean white professional
- 🌊 **Ocean** — deep blue sea
- 🌿 **Forest** — dark green nature
- 🌅 **Sunset** — warm orange/pink
- Theme saved automatically — persists across sessions

</td>
<td width="50%">

### ☁️ Cross-Device Sync
- Syncs via **private GitHub Gist** — your data, your cloud
- Works on **any browser, any device**
- Auto-saves 2 seconds after every change
- Manual sync button + auto-sync every 5 minutes
- Pulls latest data on every page load

</td>
</tr>
<tr>
<td width="50%">

### 🔒 Password Protection
- SHA-256 hashed password — never stored as plain text
- Rate limiting — 5 attempts then 30s lockout
- Lock button to secure the app anytime
- Session-based unlock — each browser is independent
- Show/hide password toggle

</td>
<td width="50%">

### 📊 Dashboard & Insights
- Daily stats — done, pending, learned, improve counts
- Progress bars for tasks and to-dos
- Work history — browse and jump to any past day
- Activity heatmap across the year
- 🔥 Day streak counter
- Summary view with total lifetime stats

</td>
</tr>
</table>

---

## 📱 Mobile vs Desktop Experience

| Feature | 📱 Mobile | 🖥️ Desktop |
|---------|--------|---------|
| Navigation | Bottom tab bar (6 tabs) | Left sidebar |
| Add Entry | Slide-up modal | Inline form + modal |
| Date picker | Compact top bar | Sidebar date nav |
| Theme switch | Mobile topbar button | Sidebar button |
| Sync | Bottom nav sync tab | Topbar sync button |
| Stats grid | 2×2 layout | 4 columns |
| Heatmap | 6 columns | 12 columns |

---

## 🎨 Theme Gallery

| Theme | Background | Accent | Feel |
|-------|-----------|--------|------|
| 🌑 Dark | `#0d0f14` | `#6c8fff` | Deep space |
| ☀️ Light | `#f5f6fa` | `#4f6ef7` | Clean minimal |
| 🌊 Ocean | `#0a1628` | `#38bdf8` | Deep sea blue |
| 🌿 Forest | `#0d1a0f` | `#4ade80` | Nature calm |
| 🌅 Sunset | `#1a0a0f` | `#fb923c` | Warm evening |

---

## 🚀 Getting Started

### 1️⃣ Open the App

```
https://dipak491.github.io/DevLog_daily_tracker/
```

### 2️⃣ Set Your Password

On first visit you'll see a welcome screen — set a password (min 4 characters).
This protects the app on that browser. You'll need it every time you open the app.

### 3️⃣ Connect GitHub Gist (for cross-device sync)

You need a **GitHub Personal Access Token** with only the `gist` scope.

<details>
<summary><b>📖 Step-by-step: Create your GitHub Token</b></summary>

<br/>

1. Go to → [github.com/settings/tokens/new](https://github.com/settings/tokens/new)
2. **Note (name):** `devlog`
3. **Expiration:** `No expiration`
4. **Scopes:** Check only ☑️ `gist` — nothing else needed
5. Click **Generate token**
6. Copy the token (starts with `ghp_`) — shown only once!
7. Paste it into the DevLog setup screen and click Connect

</details>

> 🔒 Your token is stored only in `localStorage` on your browser. Never in the repo or HTML file. Sent only to `api.github.com`.

### 4️⃣ Choose Your Theme

Click **Change Theme** in the sidebar (desktop) or **Theme** button in the topbar (mobile) to pick from 5 colour themes. Your choice is saved automatically.

---

## 🔄 How Cross-Device Sync Works

```
┌──────────────────────────────────────────────────────────┐
│                                                          │
│   📱 Mobile  ──┐                                         │
│                │                                         │
│   💻 Laptop  ──┼──► 🐙 Private GitHub Gist ◄──┐         │
│                │         (your data)            │         │
│   🖥️  Office  ──┘                               │         │
│                                                │         │
│   Any device → open URL → enter token once ───┘         │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

| What | Where it lives |
|------|---------------|
| 📝 Your data (tasks, learnings, notes) | GitHub Gist ☁️ — syncs everywhere |
| 🔑 Password hash | Browser `localStorage` — per device |
| 🔐 GitHub token | Browser `localStorage` — per device |
| 🎨 Theme preference | Browser `localStorage` — per device |
| 🌐 App code | GitHub Pages — public, static HTML |

---

## 🔐 Security Model

| Layer | Protection |
|-------|-----------|
| **App access** | Password lock screen on every new session |
| **Password storage** | SHA-256 hashed — never stored as plain text |
| **Brute force** | 5 attempts max → 30 second lockout |
| **Token scope** | `gist` only — cannot touch repos, emails, or account settings |
| **Data privacy** | Gist is **private** — invisible to everyone except you |
| **Token location** | `localStorage` only — never in the repo or HTML file |

---

## 🛠️ Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)
![GitHub Gist](https://img.shields.io/badge/GitHub%20Gist-6e40c9?style=for-the-badge&logo=github&logoColor=white)

</div>

- **Zero dependencies** — Pure HTML + CSS + Vanilla JS. No React, no npm, no build step
- **Single file** — entire app is one `index.html` — deploy anywhere in seconds
- **Storage** — `localStorage` (offline cache) + GitHub Gist API (cloud sync)
- **Security** — Web Crypto API `SHA-256` for password hashing
- **Hosting** — GitHub Pages (free, always on, no server needed)
- **Responsive** — CSS custom properties for theming, CSS Grid + Flexbox for layout
- **Fonts** — DM Serif Display · DM Mono · Syne via Google Fonts

---

## 📁 Repository Structure

```
DevLog_daily_tracker/
│
├── index.html      ← Entire app — single file, no build needed
└── README.md       ← This file
```

> The entire app is intentionally a **single HTML file** — easy to version, fork, share and deploy instantly.

---

## 🚢 Deploy Your Own Copy

```bash
# 1. Fork this repo on GitHub

# 2. Clone it locally
git clone https://github.com/YOUR_USERNAME/DevLog_daily_tracker.git
cd DevLog_daily_tracker

# 3. Enable GitHub Pages
# Go to: Settings → Pages → Source: main branch → / (root) → Save

# 4. Your app is live at:
# https://YOUR_USERNAME.github.io/DevLog_daily_tracker/
```

That's it. No npm install. No build command. No server setup. Just push and it works.

---

## 📅 Changelog

### v3.0 — Mobile + Themes Update *(Latest)*
- ✅ Fully mobile responsive with bottom navigation bar
- ✅ 5 beautiful colour themes (Dark, Light, Ocean, Forest, Sunset)
- ✅ Slide-up modals for a native mobile feel
- ✅ Compact mobile topbar and date bar
- ✅ Theme persists across sessions via localStorage
- ✅ Touch-optimized button sizes (44px+ targets)
- ✅ Mobile-friendly heatmap (6 columns on small screens)

### v2.0 — Sync + Security Update
- ✅ GitHub Gist cross-device sync
- ✅ Password lock screen with SHA-256 hashing
- ✅ Rate limiting on login attempts (5 tries → 30s lockout)
- ✅ Auto-save with 2 second debounce
- ✅ Sync status indicator in sidebar

### v1.0 — Initial Release
- ✅ Four tracking sections (Done, Todo, Learned, Improve)
- ✅ Daily notes with auto-save
- ✅ Work history browser
- ✅ Activity heatmap (12 months)
- ✅ Day streak counter
- ✅ Progress bars per section

---

## 📅 Roadmap

- [x] Daily work logging with tags
- [x] To-Do with priority levels
- [x] Learned & Improve sections
- [x] GitHub Gist cross-device sync
- [x] Password lock screen (SHA-256 hashed)
- [x] Work history browser
- [x] Activity heatmap
- [x] Day streak counter
- [x] Mobile responsive design
- [x] 5 colour themes
- [ ] Export data as PDF / CSV
- [ ] Weekly email summary
- [ ] Search across all history
- [ ] Offline PWA support (install on home screen)

---

## 👨‍💻 Author

<div align="center">

**Dipak Narkhede**

Java Developer · Spring Boot · React · Built Live PMRDA Govt. Portal · Pune, India

[![GitHub](https://img.shields.io/badge/GitHub-Dipak491-181717?style=for-the-badge&logo=github)](https://github.com/Dipak491)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-dipak--narkhede-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/dipak-narkhede)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6c8fff&height=100&section=footer&animation=fadeIn" width="100%"/>

**Built with ❤️ for developers who believe in consistency and growth**

*Log every day · Learn every day · Improve every day*

⭐ **Star this repo if it helps you stay consistent!**

</div>S
