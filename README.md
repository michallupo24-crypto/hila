# Bagrut Vocabulary Practice — מבחן אוצר מילים

A self-contained React app for Israeli high school students to practice English Bagrut vocabulary. All ~3,988 words from the six official Ministry of Education lexical bands are embedded as static data — no backend or API required.

## Local Development

```bash
npm install
npm run dev
```

## Build for Production

```bash
npm run build
# Output is in /dist — serve statically from any host
```

## Deploy to Netlify (easiest)

1. Push this repo to GitHub.
2. Go to [app.netlify.com](https://app.netlify.com) → **Add new site → Import an existing project**.
3. Connect your GitHub repo.
4. Set build settings:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
5. Click **Deploy site**. Done.

## Deploy to Vercel

1. Push this repo to GitHub.
2. Go to [vercel.com](https://vercel.com) → **Add New → Project → Import** your repo.
3. Vercel auto-detects Vite. Click **Deploy**. Done.

## Deploy to GitHub Pages

```bash
npm install --save-dev gh-pages
```

Add to `package.json` scripts:
```json
"deploy": "vite build && gh-pages -d dist"
```

Then:
```bash
npm run deploy
```

In your GitHub repo → Settings → Pages → set source to `gh-pages` branch.

> **Note for GitHub Pages:** if deploying to a sub-path (e.g. `username.github.io/repo-name`),
> add `base: '/repo-name/'` to `vite.config.js`.

## Project Structure

```
├── index.html          # Entry HTML
├── vite.config.js      # Vite config
├── package.json
├── public/
│   └── favicon.svg
└── src/
    ├── main.jsx        # React root
    └── App.jsx         # Full app + embedded vocabulary data
```
