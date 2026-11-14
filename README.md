# Prakash & Vaishnavi — Wedding Invitation

An elegant, interactive wedding invitation website, designed for guests opening a shared link on WhatsApp.

**Wedding:** 29 November 2026 · Salem · Reception on 28 November 2026

## What's inside

A single, self-contained static site — no build step, no backend, no dependencies to install.

| File | Purpose |
|------|---------|
| `index.html` | The whole site (HTML + CSS + JS, with an editable `CONFIG` object) |
| `couple.jpg` | Couple photograph |
| `ganesha.png`, `rings.png` | Ornamental motifs |
| `bokeh.jpg` | Soft fairy-light backdrop |
| `og.jpg` | Social-share preview image (1200×630) |

## Features

- Animated envelope opening (with skip + reduced-motion support)
- Couple reveal, invitation message, celebrations, live countdown, venues, and closing
- **Get Directions** (Google Maps) and **Add to Calendar** (Google Calendar + `.ics` download) for each event
- **Share** menu: WhatsApp, Instagram, Telegram, Facebook, X, Email, copy link, and the device's native share sheet
- Ambient fairy-lights, falling petals, scroll reveals, and a name shimmer — all honoring `prefers-reduced-motion`
- Fully responsive from 320px to desktop

## Editing the content

All wedding details live in one `CONFIG` object near the top of the `<script>` in `index.html`: names, dates, times, venues, maps links, and share text.

## Deploying

It's a static site — deploy the repository as-is to any static host (Vercel, Netlify, GitHub Pages).

**Vercel:** import the repo (no framework, no build command, output = root) or run `vercel` from the project folder.

After deploying, set an **absolute** URL for the social preview so WhatsApp shows the link card: in `index.html`, change the `og:image` and `twitter:image` meta tags from `og.jpg` to `https://<your-domain>/og.jpg`.
