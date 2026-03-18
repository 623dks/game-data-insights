# 🎮 Surviving the Videogame Industry

**A Data Mining Approach for Advice on Surviving the Videogame Industry**

> What do 4 million Steam reviews, 266K screenshots, and three ML models actually tell us about why some games succeed and others vanish?

This is the portfolio website for our CSCI 4502 (Data Mining) project at the University of Colorado Boulder. We pulled real data from Steam's public API, cleaned it, explored it, and ran three models on it — Association Rule Mining, CLIP, and Gradient Boosting — to find patterns that actually matter for game developers.

---

## 🔗 Live Site

Hosted on GitHub Pages — just a single `index.html` file, no build step required.

**[→ View the live site](https://www.audiovascular.com/portfolio/data-mining/introduction)**

---

## What's Inside

The site walks through the entire project from start to finish:

- **Introduction** — Why this matters. The gap between existing tools and what developers actually need.
- **Data Collection** — Three Steam API endpoints, 23,780 apps, 4.1M reviews. All sourced directly, no third-party datasets.
- **Data Cleaning** — Stripping HTML noise, handling broken descriptions, converting reviews into transaction format for mining.
- **EDA** — Visual exploration of developer/publisher performance, pricing vs. sentiment, genre distributions, and review behavior patterns.
- **Association Rule Mining** — Word co-occurrence patterns across 10 genres, split by positive and negative reviews. Story emerged as the central node in positive games.
- **CLIP (Vision-Language)** — Zero-shot genre classification from screenshots. 10/10 accuracy with no fine-tuning.
- **Gradient Boosting** — Predicting game success from image features (brightness, saturation, hue, contrast). Found that contrast 50–80 is the sweet spot and high saturation hurts.
- **Conclusions** — What it all means and where it goes next.
- **Team** — The four of us at CU Boulder.

---

## Features

| Feature | Details |
|---|---|
| **Collapsible sections** | Click any section header to collapse/expand — works like a folder system |
| **Lightbox** | Click any image to open it full-screen with blur backdrop. Press Escape or click outside to close |
| **Click to view hints** | Hover over images to see a subtle "Click to view" label |
| **Scroll animations** | GSAP-powered fade-ups, clip-path reveals, and parallax — all vertical, no zig-zag |
| **Dark theme** | Clean dark UI with blue accent, designed for readability |
| **Fully responsive** | Works on desktop, tablet, and mobile |
| **Single file** | Everything in one `index.html` — no build tools, no dependencies to install |

---

## Tech Stack

This is intentionally lightweight. No frameworks, no bundlers, no npm install.

- **HTML5** — Semantic structure, single file
- **CSS3** — Custom properties, grid, flexbox, clamp(), backdrop-filter
- **JavaScript** — Vanilla JS for accordion toggle, lightbox, nav highlighting
- **[GSAP 3.12](https://greensock.com/gsap/)** — ScrollTrigger for scroll-based animations (loaded via CDN)
- **[Google Fonts](https://fonts.google.com/)** — Space Grotesk (headings) + Inter (body)
- **Images** — Hosted externally on audiovascular.com

---

## Run Locally

It's just an HTML file. Open it directly or serve it:

```bash
# Option 1: just open the file
open index.html

# Option 2: serve with any static server
npx http-server -p 8080 -c-1
# then visit http://localhost:8080
```

No `npm install`. No `node_modules`. No `.env` files. Just open and go.

---

## Deploy to GitHub Pages

1. Push `index.html` to a GitHub repo
2. Go to **Settings → Pages**
3. Set source to your branch (e.g. `main`)
4. That's it — live in under a minute

---

## Project Structure

```
.
└── index.html    ← everything lives here
└── README.md     ← you're reading this
```

Yeah, that's it. One file. All styles are inlined in `<style>`, all scripts are inline `<script>` blocks, all images are external URLs. This was a deliberate choice — GitHub Pages serves static files, and we wanted zero friction for deployment.

---

## The Team

| Name | Role | Contact |
|---|---|---|
| **Atharva Sachin Patil** | MS Data Science | atharva.patil@colorado.edu |
| **Deep Kalpesh Shukla** | MS Data Science | deep.shukla@colorado.edu |
| **Daniel Ethridge** | PhD Student, ATLAS Institute | daniel.ethridge@colorado.edu |
| **Sujith Battu** | MS Data Science | sujith.battu@colorado.edu |

---

## Course

**CSCI 4502 · Data Mining**
University of Colorado Boulder · 2024

---

*Built with care, not with frameworks.*
