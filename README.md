# Skillbridg Learning Academy — Website

> **Learning Redefined** · Chennai's Premier Corporate Training Academy

A fully responsive, single-page marketing website for Skillbridg Learning Academy built with pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build step required.

---

## 🚀 Quick Start

```bash
# Clone or download the project
git clone https://github.com/your-org/skillbridg-website.git
cd skillbridg-website

# Open directly in browser (no server needed)
open index.html

# Or serve locally
npx serve .
# → http://localhost:3000
```

---

## 📁 Project Structure

```
skillbridg-website/
├── index.html        # Complete single-file website
├── logo.png          # Brand logo (place your file here)
└── README.md         # This file
```

> All CSS and JavaScript are embedded inside `index.html`. There are no external local dependencies beyond the logo image and a Google Fonts stylesheet (loaded via CDN).

---

## 🎨 Brand & Design Tokens

| Token | Value | Usage |
|---|---|---|
| `--deep` | `#0a052a` | Hero bg, testimonials bg, footer bg |
| `--blue` | `#029fe0` | Primary CTA, accents, stats band |
| `--blue-h` | `#00b8ff` | Button hover state |
| `--white` | `#ffffff` | Light section backgrounds |
| `--off` | `#f4f9fd` | Alternate section tint |
| `--ink` | `#0e1a30` | Body text |

**Fonts** (loaded from Google Fonts):
- **DM Serif Display** — headings & display numbers
- **DM Sans** — all body copy, labels, navigation

---

## 📄 Page Sections

| # | Section | ID | Background |
|---|---|---|---|
| 1 | Navigation | `#nav` | White / fixed |
| 2 | Hero | `#hero` | White |
| 3 | Sector Ticker | `#tkr` | Off-white |
| 4 | Services | `#services` | White |
| 5 | Approach | `#approach` | Off-white |
| 6 | Why Skillbridg | `#why` | White |
| 7 | Testimonials | `#testi` | `#0a052a` dark |
| 8 | Stats Band | `#sband` | `#029fe0` blue |
| 9 | Contact | `#contact` | White |
| 10 | Footer | `footer` | `#0a052a` dark |

---

## ✏️ Common Customizations

### Update contact details
Search for the following strings in `index.html` and replace:

```
info@skillbridglearningacademy.in   → your email
+91 91765 43210                     → your phone number
Chennai, Tamil Nadu, India          → your location
```

### Swap the logo
Replace `logo.png` in the project root with your logo file (recommended height: **40px**, any width). The `<img>` tag references `logo.png` in both the nav and footer.

### Change the hero headline
Find the `<h1 class="hh1">` tag and update the text:

```html
<h1 class="hh1">
  Transform<br>
  Your Workforce.<br>
  <em>Redefine Learning.</em>   <!-- em = italic blue accent -->
</h1>
```

### Update stats numbers
Find the `#sband` section and edit the `.scn` values:

```html
<div class="scn">500<span>+</span></div>   <!-- Corporates Trained -->
<div class="scn">50<span>K+</span></div>   <!-- Professionals Impacted -->
<div class="scn">12<span>+</span></div>    <!-- Years of Excellence -->
<div class="scn">4<span>+</span></div>     <!-- South Indian Cities -->
```

### Update social media links
Search for `https://linkedin.com`, `https://instagram.com`, etc. and replace with your actual profile URLs.

### Add or remove a service row
Each service is a `.svr` block inside `.svl`. Copy and paste a block, then update the number, icon, title, description, and tags:

```html
<div class="svr">
  <div class="svnum">06</div>
  <div class="svb">
    <div class="svic">🎤</div>
    <div class="svt">
      <h3>Your New Service</h3>
      <p>Description of the service goes here.</p>
      <div class="svtags">
        <span class="svtag">Tag One</span>
        <span class="svtag">Tag Two</span>
      </div>
    </div>
  </div>
  <div class="svarr">→</div>
</div>
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout changes |
|---|---|
| `≤ 1024px` | Reduced padding, tighter footer columns |
| `≤ 900px` | Mobile nav (hamburger), hero panel hidden, all grids stack |
| `≤ 640px` | Full-width buttons, single-column testimonials, simplified stats |
| `≤ 380px` | Minimum font sizes, fully stacked stats grid |

---

## ⚙️ JavaScript Features

All JS is vanilla, no libraries required.

| Feature | Description |
|---|---|
| Mobile nav | Hamburger toggle with body scroll lock |
| Nav shadow | Box-shadow added on scroll past 40px |
| Scroll reveal | `IntersectionObserver` fades elements in on scroll |
| Smooth anchors | All `href="#section"` links scroll with nav offset compensation |
| Counter animation | Stats band numbers count up with eased animation on first view |
| Sector ticker | CSS `@keyframes` animation, pauses on hover |

---

## 🌐 Deployment

The site is a single static file and can be deployed anywhere:

**Netlify (drag & drop)**
1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the project folder onto the deploy zone

**GitHub Pages**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-org/skillbridg-website.git
git push -u origin main
# Enable Pages in repo Settings → Pages → Branch: main
```

**Vercel**
```bash
npx vercel
```

---

## 🔗 External Dependencies (CDN only)

| Resource | URL | Purpose |
|---|---|---|
| DM Serif Display | fonts.googleapis.com | Display headings |
| DM Sans | fonts.googleapis.com | Body & UI text |

No npm packages. No build tools. No JavaScript frameworks.

---

## 📋 Browser Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| IE 11 | ❌ Not supported |

---

## 📝 License

© 2026 Skillbridg Learning Academy · All rights reserved.  
This codebase is proprietary. Do not redistribute without written permission.

---

*Built with HTML · CSS · Vanilla JS — no frameworks, no build steps, just the web.*
