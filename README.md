# Mosso Website

Static website for Mosso — a daily puzzle mobile app by DataNaat.

Live at: https://mosso.day

## Structure

```
.
├── index.html        Landing page
├── privacy.html      Privacy Policy
├── terms.html        Terms of Service
├── support.html      Support / FAQ
├── 404.html          Not Found error page
├── style.css         All styling (paper-zen design system)
├── assets/
│   ├── icon.png      App icon (Mosso M, Pine Blue on Celadon)
│   ├── wordmark.png  Wordmark on Celadon background
│   └── wordmark_dark.png  Wordmark on Space Indigo background
└── README.md
```

## Local preview

Open `index.html` directly in any browser. No build step required — pure HTML/CSS.

```bash
# Optional: serve via simple HTTP server
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Deploy

Hosted on Vercel. Auto-deploys on push to `main`.

Custom domain `mosso.day` is configured in Cloudflare DNS pointing to Vercel.

## Update guidelines

- **Privacy / Terms changes:** update the "Last updated" date at the top of each page.
- **New features in app:** add a feature card to `index.html` features grid.
- **New language:** the website is intentionally English-only. The app itself supports 5 languages.

## Tech

- Pure HTML5 + CSS3, no JavaScript.
- Fonts: Fraunces (display) + Inter (body) from Google Fonts.
- Dark mode supported via `prefers-color-scheme`.
- Mobile-responsive.
- Lighthouse score: 100/100/100/100 expected.

## License

© 2026 DataNaat. All rights reserved.
