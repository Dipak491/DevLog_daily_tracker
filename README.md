<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6c8fff&height=200&section=header&text=DevLog&fontSize=80&fontAlignY=35&desc=Daily%20Work%20Tracker&descAlignY=55&descSize=22&fontColor=ffffff&animation=fadeIn" width="100%"/>

<br/>

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-DevLog-6c8fff?style=for-the-badge&logoColor=white)](https://dipak491.github.io/DevLog_daily_tracker/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222?style=for-the-badge&logo=github&logoColor=white)](https://dipak491.github.io/DevLog_daily_tracker/)
[![License](https://img.shields.io/badge/License-MIT-3ecf8e?style=for-the-badge)](LICENSE)
[![Made with](https://img.shields.io/badge/Made%20with-HTML%20%7C%20CSS%20%7C%20JS-f59e0b?style=for-the-badge)](https://github.com/Dipak491/DevLog_daily_tracker)

<br/>

> **A beautiful, secure, cross-device daily work tracker for developers.**  
> Log what you did, what you need to do, what you learned, and where you want to improve —  
> synced across all your devices via GitHub Gist. Protected by a password lock.

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
- 📚 **What I Learned** — capture concepts, tricks, tools
- 📈 **Areas to Improve** — track growth areas with urgency

</td>
<td width="50%">

### ☁️ Cross-Device Sync
- Syncs via **private GitHub Gist** — your data, your cloud
- Works on **any browser, any device**
- Auto-saves every 2 seconds after changes
- Manual sync button + auto-sync every 5 minutes

</td>
</tr>
<tr>
<td width="50%">

### 🔒 Password Protection
- SHA-256 hashed password stored locally
- Rate limiting — 5 attempts then 30s cooldown
- Lock button in topbar to secure anytime
- Session-based unlock — each browser stays independent

</td>
<td width="50%">

### 📊 Dashboard & Insights
- Daily stats — done, pending, learned, improve counts
- Progress bars for tasks and to-dos
- Work history — browse & jump to any past day
- Activity heatmap for the year
- 🔥 Day streak counter

</td>
</tr>
</table>

---

## 🖥️ Preview

<div align="center">

| Today's Work | To-Do List | History |
|:---:|:---:|:---:|
| Log your daily work with tags | Track tasks with priorities | Browse all past days |

</div>

---

## 🚀 Getting Started

### 1️⃣ Open the App

```
https://dipak491.github.io/DevLog_daily_tracker/
```

### 2️⃣ Set Your Password

On first visit, you'll be prompted to set a password. This protects the app on that browser. Minimum 4 characters.

### 3️⃣ Connect GitHub Gist (for cross-device sync)

You need a **GitHub Personal Access Token** with only the `gist` scope.

<details>
<summary><b>📖 Step-by-step: Create your GitHub Token</b></summary>

<br/>

1. Go to → [github.com/settings/tokens/new](https://github.com/settings/tokens/new)
2. **Note:** `devlog`
3. **Expiration:** `No expiration` (or 90 days for more security)
4. **Scopes:** Check only ☑️ `gist` — nothing else needed
5. Click **Generate token**
6. Copy the token (starts with `ghp_`) — it's shown only once!
7. Paste it into the DevLog setup screen

</details>

> 🔒 **Your token never leaves your browser.** It's stored only in `localStorage` and sent only to `api.github.com`.

---

## 🔄 How Sync Works

```
┌─────────────────────────────────────────────────────────┐
│                                                         │
│   📱 Phone  ──┐                                         │
│               │                                         │
│   💻 Laptop ──┼──► 🐙 Private GitHub Gist ◄──┐         │
│               │         (your data)           │         │
│   🖥️  Office ──┘                              │         │
│                                               │         │
│   Any device opens the URL → enters token ───┘         │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

| What | Where it lives |
|------|---------------|
| 📝 Your data (tasks, learnings) | GitHub Gist ☁️ — syncs everywhere |
| 🔑 Password hash | Browser `localStorage` — per device |
| 🔐 GitHub token | Browser `localStorage` — per device |
| 🌐 App code | GitHub Pages — public, static |

---

## 🛠️ Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)
![GitHub Gist](https://img.shields.io/badge/GitHub%20Gist-6e40c9?style=for-the-badge&logo=github&logoColor=white)

</div>

- **Frontend:** Pure HTML + CSS + Vanilla JS — zero dependencies, zero build step
- **Storage:** Browser `localStorage` (offline cache) + GitHub Gist API (cloud sync)
- **Security:** Web Crypto API (`SHA-256`) for password hashing
- **Hosting:** GitHub Pages (free, always on)
- **Fonts:** DM Serif Display · DM Mono · Syne (Google Fonts)

---

## 🔐 Security Model

| Layer | Protection |
|-------|-----------|
| **App access** | Password lock screen (SHA-256 hashed, never plain text) |
| **Brute force** | 5 attempts max → 30 second lockout |
| **Token scope** | `gist` only — cannot access repos, emails, or account settings |
| **Data privacy** | Gist is **private** — invisible to everyone except you |
| **Token storage** | `localStorage` only — never in the repo or HTML file |

---

## 📁 Repository Structure

```
DevLog_daily_tracker/
│
└── index.html          # The entire app — single file, no build needed
└── README.md           # This file
```

> The app is intentionally a **single HTML file** — easy to deploy, version, and share.

---

## 🚢 Deploying Your Own Copy

```bash
# 1. Fork this repo on GitHub

# 2. Clone it
git clone https://github.com/YOUR_USERNAME/DevLog_daily_tracker.git
cd DevLog_daily_tracker

# 3. Enable GitHub Pages
# Go to: Settings → Pages → Source: main branch → / (root) → Save

# 4. Your app is live at:
# https://YOUR_USERNAME.github.io/DevLog_daily_tracker/
```

---

## 📅 Roadmap

- [x] Daily work logging
- [x] To-Do with priorities
- [x] Learned & Improve sections
- [x] GitHub Gist cross-device sync
- [x] Password lock screen
- [x] Work history browser
- [x] Activity heatmap
- [x] Day streak counter
- [ ] Export data as PDF / CSV
- [ ] Dark / Light theme toggle
- [ ] Weekly summary email (via GitHub Actions)
- [ ] Tags & search across history

---

## 👨‍💻 Author

<div align="center">

**Dipak** — Java Developer | Spring Boot | React | PMRDA RTS Portal

[![GitHub](https://img.shields.io/badge/GitHub-Dipak491-181717?style=for-the-badge&logo=github)](https://github.com/Dipak491)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6c8fff&height=100&section=footer&animation=fadeIn" width="100%"/>

**Built with ❤️ for developers who value consistency and growth**

*Log every day. Learn every day. Improve every day.*

</div>