<div align="center">

# 🏆 Premium Validator | GG Mouse Pro

![GG Mouse Pro Premium Validator](https://files.catbox.moe/hcyo4l.jpg)

**Official Premium Check Tool for GG Mouse Pro**

[![Status](https://img.shields.io/badge/status-active-success.svg)](https://check-status-xi.vercel.app/)
[![Made with](https://img.shields.io/badge/made%20with-HTML%20%7C%20Tailwind%20CSS%20%7C%20JS-38bdf8.svg)]()
[![Tailwind CSS](https://img.shields.io/badge/styled%20with-Tailwind%20CSS-06b6d4?logo=tailwind-css&logoColor=white)]()
[![Vercel](https://img.shields.io/badge/deployed%20on-vercel-black.svg)](https://vercel.com/)

</div>

---

## 📋 Overview

**Premium Validator** is the official web-based verification dashboard for **GG Mouse Pro** — allowing teams and users to instantly validate premium account status, verify subscriptions, and search active order details using just an email or order ID.

## ✨ Features

- **Premium Account Check** — Validate any user's active premium subscription by email
- **Order Status Lookup** — Fetch days, email, expiry and purchase date by Order ID (GPA format)
- **Auto-Clipboard Copy** — Email auto-copied after order lookup + shown in a plain info box
- **Fully Responsive** — Works on mobile, tablet and desktop
- **Instant Results** — 10-second timeout for fast feedback
- **Secure & Direct** — Production-ready Vercel proxy to avoid Mixed Content / CORS
- **Clean Product UI** — Built with Tailwind CSS. Solid card layout, brand palette, no visual noise
- **Accessible Form Labels** — Proper `<label for>` bindings, focused focus rings, readable contrast
- **Plain Language Copy** — No emoji spam, no over-the-top marketing — just a tool that does what it says

## 🚀 Live Demo

👉 **Check Now**: [https://check-status-xi.vercel.app/](https://check-status-xi.vercel.app/)

---

## 🛠️ How to Use

### 1️⃣ Check Premium Account

1. Enter the user's **email address** in the first input field
2. Click **"Paste"** to paste from clipboard or type manually
3. Click **"Check Premium"**
4. See instant result: `The user is premium!!` or `Not premium :(`

### 2️⃣ Check Order Details

1. Enter the **Order ID** (starts with `GPA.` e.g. `GPA.1234-5678`)
2. Click **"Paste"** or type the order ID
3. Click **"Check Order"**
4. You'll receive:
   - Days of premium subscription
   - Credit account email
   - Current subscription expire time
   - Purchase date
   - **Email auto-copied to clipboard** ✨

---

## 🏗️ Tech Stack

| Frontend | Purpose |
|----------|---------|
| HTML5 | Structure & Semantics |
| **Tailwind CSS 3** | Utility-first framework for modern responsive design |
| Custom CSS (`naagin.css`) | Loader animation + button / input base styles |
| Vanilla JS | Core logic, clipboard, and dynamic UI updates |
| jQuery | AJAX API calls |
| Vercel | Deployment & API proxying |

### 🎨 Tailwind CSS Highlights
- **Custom `gmp` color palette**: Brand purples tied to GG Mouse Pro identity
- **Layout**: Plain white product card over a subtle gradient background
- **Forms**: Accessible `<label>` tags, gray-50 inputs that go white on focus, brand-colored focus ring
- **Buttons**: Two-tone visual weight (gray secondary + solid purple primary), no hover-lift gimmicks
- **Typography**: Inter font stack, grounded sizes (14-15px body copy), uppercase micro-label in header

## 📁 Project Structure

```
Check-Status-main/
├── index.html       # Main HTML page (meta tags + UI + JS logic)
├── naagin.css       # Custom stylesheet (Uiverse.io inspired)
├── vercel.json      # Vercel proxy configuration
└── README.md        # This file
```

## 🔌 API Integration

The app dynamically selects the API base URL based on environment:

```
✅ Localhost/LAN  → http://api.gmp.jyyxt.online
✅ Production     → Relative path (proxied via vercel.json)
```

### Endpoints Used

| Method | Endpoint | Purpose |
|--------|----------|---------|
| GET | `/api/v3/users/is_premium/{email}` | Check if user has premium |
| GET | `/api/v3/orders/{orderId}` | Fetch complete order details |

---

## 🎨 Preview Banner

![Banner Preview](https://files.catbox.moe/hcyo4l.jpg)

> *Banner URL: `https://files.catbox.moe/hcyo4l.jpg` — Used as `og:image` for SEO & social sharing.*

---

## 🔍 SEO & Metadata

This project includes comprehensive SEO optimization:

- ✅ **80+ Keywords** (premium validator, gg mouse pro premium check, gg premium check, etc.)
- ✅ **Open Graph (OG) Tags** — Rich social share previews
- ✅ **Twitter Card** — Summary large image card
- ✅ **Google Site Verification**
- ✅ **Theme Color** meta tag
- ✅ **Robots / Language / Revisit-After** tags

---

## 🔧 Local Development

1. Clone / download the project
2. Open `index.html` directly in a browser, OR
3. Serve locally using any static server:
   ```bash
   npx serve .
   # or
   python -m http.server 8000
   ```
4. Visit `http://localhost:8000`

---

## 🚀 Deployment

One-click deploy to **Vercel**:

```bash
# 1. Install Vercel CLI
npm i -g vercel

# 2. Deploy
vercel
```

The `vercel.json` config automatically proxies API calls to avoid Mixed Content / CORS issues in production.

---

## 🤝 Contributing

Powered by [GG Mouse Pro](https://www.ggmousepro.in/) — official project. For issues, reach out to the GG Mouse Pro team.

---

<div align="center">

**Made with ❤️ for the GG Mouse Pro Community**

[![GG Mouse Pro](https://img.shields.io/badge/GG%20Mouse%20Pro-Official-blue.svg)](https://www.ggmousepro.in/)

</div>
