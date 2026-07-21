# Se1Schools2027 — Year 7 school shortlist (Sept 2027)

Interactive comparison for home postcode **SE17 1BS**.

## Sharing: public vs private repo

| Hosting | Need public GitHub repo? |
|--------|---------------------------|
| **GitHub Pages (free, personal account)** | **Yes** — free Pages for user sites requires a public repo |
| **GitHub Pages (Pro/Team)** | No — private Pages allowed on paid plans |
| **Netlify / Cloudflare Pages free** | No — can deploy from a private repo; share the deploy URL |
| **Multi-user ranking/checklist (JSONBlob)** | Independent of GitHub visibility — works as long as people open the same site URL |

So: **for free GitHub Pages sharing, the repo must stay public.** If you want a private code repo, host the static site elsewhere (Netlify/Cloudflare) and share that URL instead.

## Live site

- Pages: https://pfaisant.github.io/Se1Schools2027/ (after rename) or previous Pages URL until DNS updates
- Repo: https://github.com/pfaisant/Se1Schools2027

## Features

- Preference ranking (▲▼) shared live with anyone who has the public link
- Shared checklist / plan ticks
- Sortable tables, column tooltips, fees colour scale
- Comments feed for feedback
- Autosave (no save button)

## Local open

Use a static server (needed for `fetch` of `sync-config.json`):

```bash
cd D:\louis-year7-2027
npx --yes serve -p 5173
```

Opening `index.html` via `file://` may break autosave/sync (browser security).
