<div align="center">

<img src="icons/icon.png" alt="SchoolPulse" width="100" height="100">

# 🌐 SchoolPulse — Official Website

**The official landing page for SchoolPulse app.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](#-license)

[🌍 Visit Live](https://motechorbit.github.io/SchoolPulse/)

</div>

---

## 📖 About

The official website of **SchoolPulse** — a smart offline school assistant app for students. The site features a cinematic 3D intro, detailed feature showcase, and direct download links.

---

## ✨ Features

- 🎬 **Cinematic 3D Intro** — Rocket flies in, crashes, debris forms "SchoolPulse"
- 🌙 **Dark / Light Mode** — Auto-detects system preference
- 📱 **Fully Responsive** — Works on mobile, tablet, desktop
- ⚡ **Fast & Lightweight** — No frameworks, pure HTML/CSS/JS
- 🔒 **Offline-Ready** — No external API calls (except CDN for icons)
- 🎨 **Material 3 Design** — Matches the app's visual identity
- 🔍 **SEO Optimized** — Full Open Graph, Twitter Cards, Schema.org

---

## 📁 Project Structure

```
schoolpulse-website/
├── index.html              # Main page (with cinematic intro)
├── admin.html              # Exams & feedbacks dashboard
├── manifest.json           # PWA manifest
├── robots.txt              # SEO
├── sitemap.xml             # SEO
├── README.md               # This file
│
├── icons/
│   ├── icon.png            # Main logo (512×512)
│   ├── icon-32.png
│   ├── icon-96.png
│   ├── icon-144.png
│   ├── icon-180.png
│   ├── icon-192.png
│   ├── icon-512.png
│   ├── preview.png         # Social share (1200×630)
│   ├── student.png         # About App section
│   └── dev-icon.png        # About Developer section
│
└── screenshots/            # Optional app screenshots
    ├── home.png
    ├── timetable.png
    ├── alarms.png
    └── settings.png
```

---

## 🎬 Cinematic Intro

When visitors open the site, they see:

1. **Rocket flies in** from off-screen (3D perspective)
2. **Impact & explosion** — camera shakes & flips
3. **Debris flies** in all directions
4. **Letters "SchoolPulse"** form from the debris
5. **"V2.0.0"** appears
6. **Auto-transition** to main site

**Duration**: ~6 seconds. No skip button — pure cinematic experience.

---

## 🛠️ Customization

### Change Version Number

Search in `index.html` for:
```html
<span class="version-badge">الإصدار 2.0.0</span>
<span class="sp3d__chip">● V2.0.0</span>
```

### Change Download Link

```html
<a href="https://your-download-link.com" class="download-btn download-btn-primary">
  تحميل APK مباشر
</a>
```

### Change Developer Info

```html
<h3>Mohamed Hany</h3>
<a href="tel:01553308975">01553308975</a>
```

### Admin Dashboard (Admin.html)

The `admin.html` file provides a dashboard to manage:
- **Exams** — Add/delete exams shown in the app
- **Feedbacks** — View/delete user feedbacks

**Access**: Opens with password (default: `schoolpulse2026`).

**Backend**: [JSONBin.io](https://jsonbin.io) — Free cloud storage.

#### JSONBin Structure

```json
{
  "exams": [],
  "feedbacks": []
}
```

To change the bin, edit in `admin.html`:
```javascript
const BIN_ID = 'your-bin-id';
const MASTER_KEY = 'your-master-key';
```

---

## 🚀 Deployment

### Option 1: GitHub Pages (Recommended)

1. Push to a GitHub repository.
2. **Settings** → **Pages** → **Source**: `main` branch.
3. Wait 1-2 minutes.
4. Site is live at `https://username.github.io/repo-name/`.

### Option 2: Netlify Drop

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag the folder.
3. Get instant link.

### Option 3: Vercel

```bash
npm i -g vercel
vercel
```

---

## 🔧 Local Development

Just open `index.html` in a browser. No build step required.

**For local server**:
```bash
# Python
python -m http.server 8000

# Node.js
npx serve
```

Then open `http://localhost:8000`.

---

## 📱 PWA (Progressive Web App)

The site can be installed as a standalone app:

- **Android**: Chrome → menu → "Install app"
- **iOS**: Safari → Share → "Add to Home Screen"
- **Desktop**: Chrome → install icon in address bar

Requirements:
- `manifest.json` ✅
- HTTPS ✅ (required by browsers)
- Icons (192, 512) ✅

---

## 🔒 Security

- ✅ No user data collection.
- ✅ No third-party analytics.
- ✅ HTTPS enforced via GitHub Pages.
- ⚠️ **Admin.html** contains JSONBin credentials — **do not share publicly**.

---

## 📝 License

```
© 2026 Mohamed Hany. All rights reserved.
```

This project is **proprietary** and may not be copied, distributed, or modified without written permission.

---

## 👨‍💻 Developer

**Mohamed Hany**

📞 01553308975 | 01553308947

© 2026 Mohamed Hany. All rights reserved.

