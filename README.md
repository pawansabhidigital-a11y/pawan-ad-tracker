# Ad Account Manager

Single self-contained page (`index.html`) — no build step needed. Combines:
- **Account Setup** (Ad Account ID, Pixel ID, Access Token, Audience Exclusion, Video/Image ADS, Ads From Client, Pages)
- **Tracking** (Priority, Checked, Date Checked, Optimization Done, Status, Update/Remarks)
- **Landing Pages** overview — every page across every client in one table

## Deploy to Vercel

**Option A — Vercel CLI**
```
npm i -g vercel
cd ad-account-manager
vercel --prod
```

**Option B — Drag and drop**
1. Go to https://vercel.com/new
2. Select the files **inside** this folder (index.html, vercel.json, README.md) — not the folder itself — and drag them in.

**Option C — GitHub**
1. Push the contents of this folder to the ROOT of a new GitHub repo (index.html must sit at the repo root, not in a subfolder).
2. On vercel.com, "Add New Project" → import that repo → Deploy.

## Notes
- All data is saved in the browser's local storage on your device — nothing is sent anywhere, no backend needed.
- Click a client on the left to see/edit their accounts (Setup + Tracking). Click "Landing Pages" to see every page across all clients.
- Access Token fields are masked by default — click "Show" to reveal.
- "Reset data" isn't built in by default; to start fresh, clear this site's local storage from your browser's dev tools.
