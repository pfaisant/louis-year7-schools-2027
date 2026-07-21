# Louis — Year 7 school shortlist (Sept 2027)

Interactive comparison for home postcode **SE17 1BS**.

## Features

- Preference ranking (▲▼) shared live with anyone who has the public link
- Shared checklist (multi-user, no login)
- Sortable main + alternatives tables
- Commute **> 40 minutes** highlighted in scarlet
- CdG international options (French / SI–BFI / British Section)
- No girls’ schools on the alternatives list

## Multi-user sync

1. Browser loads `sync-config.json` → cloud blob id  
2. Ranking + checklist read/write via JSONBlob (`PUT`/`GET`)  
3. Everyone on the public URL polls every ~4s  
4. GitHub Action `.github/workflows/sync-keepalive.yml` refreshes the blob every 8h and backs up to `state.json`

## Local open

Open `index.html` via a local static server (needed for `fetch` of `sync-config.json`):

```bash
cd D:\louis-year7-2027
npx --yes serve -p 5173
```

## GitHub Pages

After the repo is public and Pages is enabled (branch `main` / root):

`https://<user>.github.io/<repo>/`
