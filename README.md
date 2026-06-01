# Kennedy Maingi — Security Portfolio

**Live URL:** `https://YOUR-GITHUB-USERNAME.github.io/portfolio`

Personal portfolio website for Kennedy Maingi — Penetration Tester & Bug Bounty Hunter. Built as a single-file HTML/CSS/JS site, hosted free on GitHub Pages.

## Features
- Auto-updating age (calculates from Dec 12, 2002 on every visit)
- Animated terminal typewriter for roles
- Blog, Projects, Certifications & Education sections
- Drag-and-drop file upload UI
- Newsletter subscription via Web3Forms (free)
- Contact form via Formspree (free)
- Fully responsive (mobile + desktop)
- Zero dependencies, no build step

## Quick Setup

### 1. Get your free form keys

**Contact Form → Formspree (free, 50 submissions/month)**
1. Go to https://formspree.io → Sign up free
2. Click "New Form" → name it "Portfolio Contact"
3. Copy the form ID (looks like `xpwzabcd`)
4. Open `index.html`, find `YOUR_FORMSPREE_ID` and replace it

**Newsletter → Web3Forms (free, 250 submissions/month)**
1. Go to https://web3forms.com → Enter your email → Get free key
2. Open `index.html`, find `YOUR_WEB3FORMS_KEY` and replace it

### 2. Deploy to GitHub Pages (free hosting)

**Option A — Via GitHub website (easiest):**
1. Go to https://github.com → Sign in (or create account)
2. Click **"New repository"** (green button)
3. Name it exactly: `portfolio` (or `YOUR-USERNAME.github.io` for root URL)
4. Set to **Public** → Click **"Create repository"**
5. Click **"uploading an existing file"** link
6. Drag and drop `index.html` and `README.md` → Click **"Commit changes"**
7. Go to **Settings** → **Pages** (left sidebar)
8. Under "Source" → select **"Deploy from a branch"**
9. Branch: `main` | Folder: `/ (root)` → Click **Save**
10. Wait ~2 minutes → Your site is live at `https://YOUR-USERNAME.github.io/portfolio`

**Option B — Via Git CLI:**
```bash
git init
git add .
git commit -m "Initial portfolio launch 🚀"
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
git push -u origin main
# Then enable Pages in repo Settings → Pages
```

### 3. Personalise your content

Open `index.html` and update:

| What to change | Search for |
|---|---|
| Email address | `kennedy@maingisec.com` |
| Social links | `Twitter/X`, `LinkedIn`, `GitHub` (add your real URLs) |
| Blog posts | `<!-- BLOG -->` section |
| Projects | `<!-- PROJECTS -->` section |
| Certifications | `<!-- CERTS -->` section |
| Stats (bugs, bounties) | `hero-stats` section |
| Your photo/avatar | Replace `KM` initials in `.avatar-wrap` with an `<img>` tag |

### 4. Custom domain (optional, free)

If you have a domain (e.g. `maingisec.com`):
1. In GitHub repo → Settings → Pages → Custom domain → enter your domain
2. At your domain registrar, add a CNAME record: `www` → `YOUR-USERNAME.github.io`

## File Structure
```
portfolio/
├── index.html   ← entire site (HTML + CSS + JS in one file)
└── README.md    ← this file
```

## Tech Stack
- Pure HTML5 / CSS3 / Vanilla JS — no frameworks, no build tools
- Fonts: Syne + Share Tech Mono + DM Sans (Google Fonts CDN)
- Forms: Formspree + Web3Forms (both free tiers)
- Hosting: GitHub Pages (free, unlimited bandwidth for static sites)
