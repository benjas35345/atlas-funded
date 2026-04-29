# Atlas Funded — Vercel demo

Static, single-file demo of the Atlas Funded Risk Operations review system. Drag this folder onto Vercel (or run `vercel --prod`) and you have a live URL in 60 seconds.

## Deploy in one command

```bash
cd atlas-funded-vercel-demo
npx vercel --prod
```

You'll be prompted to log in (GitHub / GitLab / email), confirm the project name, and Vercel returns a `https://<name>.vercel.app` URL. No build step, no backend, no env vars. The whole app is one HTML file.

## Or deploy via the dashboard

1. Zip this folder.
2. Go to https://vercel.com/new
3. Drag the zip onto the upload area.
4. Click **Deploy**.

## Or via GitHub

1. `git init && git add . && git commit -m "Atlas Funded demo"`
2. Push to a new GitHub repo.
3. https://vercel.com/new → import that repo → Deploy.

## What's in here

- `index.html` — the entire app, self-contained. State lives in browser memory.
- `vercel.json` — minimal config: clean URLs + sensible security headers.

## What it is and isn't

This is the **demo**, not the production app. It's the same UI, the same workflow, the same brand identity, the same engine logic — but state is in-memory only. No Postgres, no R2, no auth. Use it to show the team and stakeholders what the production system looks like and feels like.

For the **production** Next.js app (real database, real file storage, real auth, real audit trail), see `../atlas-funded-risk/README.md`.
