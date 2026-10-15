# Leo & Roan — Accountability Tool

Internal dashboard for our Pinterest coaching business.

## Features
- **Overview** — total collected, next milestone, revenue trend (7 days / this month / last month / 6 months), upcoming payments, activity feed
- **Revenue** — adjustable goal ($900k default), custom milestones, collected-by-client breakdown
- **Clients** — package price, installments, amount paid/due, next payment, status, join date, notes
- **Accountability** — posting log per partner, weekly goal, streaks, 18-week heatmap
- **Notes** — shared ideas & coaching notes, pin important ones
- **To-Do's** — tasks with assignee (Leo / Roan / Both), tracks who completed what
- **Resources** — client video library (Loom / Vimeo), filter by Pinterest / Shopify / Backend
- **Client Progress** — stage tracker per client (Onboarding → Website → Pinterest → Backend → Complete)
- **Affiliate Deals** — links, discount codes, commissions

## Deploy (GitHub Pages)
1. Create a new repository on GitHub (private is fine for the code, but note Pages sites are public unless you're on a paid org plan).
2. Upload `index.html` and `README.md` to the repo root.
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After ~1 minute your tool is live at `https://<your-username>.github.io/<repo-name>/`.

Alternatives: drag `index.html` into [Netlify Drop](https://app.netlify.com/drop) or import the repo into Vercel — no build step needed.

## Important: where data is stored
All data is saved in **your browser's localStorage**. That means:
- Data is **per browser, per device**. Leo's laptop and Roan's laptop will **not** see each other's entries.
- Clearing browser data deletes everything.
- There is **no password** — anyone with the URL can open the tool (they'd see an empty/demo dashboard, not your data, since data lives in your browser).

For a shared, synced dashboard you'd need a backend (e.g. Supabase or Firebase) — a future upgrade.

## Updating
Replace `index.html` in the repo with a new export and commit. Your saved data stays in your browser.
