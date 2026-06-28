# Bagrut Vocabulary Practice — מבחן אוצר מילים

React app for practicing English Bagrut vocabulary. All ~4,156 words from the six official Ministry of Education lexical bands are embedded as static data — no backend required.

## Run locally

```bash
npm install
npm run dev
```

## Deploy to Netlify

1. Push this repo to GitHub
2. [app.netlify.com](https://app.netlify.com) → Add new site → Import from GitHub
3. Build command: `npm run build` | Publish directory: `dist`
4. Deploy

## Deploy to Vercel

1. Push to GitHub
2. [vercel.com](https://vercel.com) → New Project → Import
3. Vercel auto-detects Vite → Deploy

## Deploy to GitHub Pages

```bash
npm install --save-dev gh-pages
# Add to package.json scripts: "deploy": "vite build && gh-pages -d dist"
npm run deploy
```

> If deploying to a sub-path, add `base: '/repo-name/'` to `vite.config.js`.
