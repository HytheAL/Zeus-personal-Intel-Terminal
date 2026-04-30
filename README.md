# ZEUS — Personal Intelligence Terminal

A self-contained personal life OS dashboard. Three tabs: **Command** (markets + trade desk + news), **Athlete** (workout + BJJ + nutrition), **Scout** (vintage watch + clothing hunting).

## Deploy to Vercel via GitHub

1. Push this repository to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import Git Repository
3. Select this repo → click **Deploy** (zero configuration needed)
4. Your ZEUS terminal will be live at `https://your-project-name.vercel.app`

## First Launch

When you open ZEUS for the first time, you'll be prompted to enter your **Anthropic API key**.

- Your key is stored in `localStorage` — it never leaves your browser
- It powers the AI Workout Refresh button and live news feed
- To reset the key, click the `API ●` button in the top bar

## Features

- **ALD × Porsche colour system** — deep forest green canvas, near-black obsidian panels, varsity gold accents
- **Command Tab** — live EUR/USD chart, SMC checklist, macro news feed, equity tracker (add your own tickers)
- **Athlete Tab** — full 5-day PPL workout programme, BJJ session log, macro rings, food logger with hawker database
- **⚡ AI Workout Refresh** — one click generates a completely new, research-backed workout programme via Claude API
- **Scout Tab** — vintage watch + clothing deal alerts, hunt list, platform scan links, price alert setter
- **DEMO / LIVE mode toggle** — switch between mock data and live API calls
- **Fully persistent** — API key, tickers, priorities, SMC levels, food log all saved to localStorage

## Tech Stack

- Pure HTML/CSS/JS — no build step, no npm, no frameworks
- Chart.js 4.4.0 (CDN)
- Google Fonts: Cormorant Garamond + DM Mono
- Anthropic Claude API (claude-sonnet-4-20250514) for AI features
- Frankfurter API for EUR/USD (free, no key needed)
- Hosted on Vercel as a static file

## Files

```
index.html    — The complete ZEUS dashboard (single file)
vercel.json   — Vercel deployment configuration
README.md     — This file
.gitignore    — Excludes build artifacts
```
