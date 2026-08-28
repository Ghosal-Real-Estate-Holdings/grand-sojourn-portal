# Grand Sojourn Room Block Portal

Static, self-contained room-block lookup tool for The Grand Sojourn, hosted on GitHub Pages at
`portal.ghosalexperiences.com/the-grand-sojourn/`.

- `the-grand-sojourn/index.html` — the whole app (couple lookup + admin panel), no build step.
- `the-grand-sojourn/grand-sojourn.json` — the data it reads. Guests fetch this directly.

## Updating reservation data

1. Open the portal, click **Venue team login**, sign in with the admin passcode.
2. Import your reservation export (.xlsx) or edit reservations directly, then click
   **Download updated file** — this downloads a new `grand-sojourn.json`.
3. In this repo, replace `the-grand-sojourn/grand-sojourn.json` with the downloaded file
   (GitHub web UI: open the file → pencil icon → upload, or drag-and-drop via
   **Add file → Upload files**) and commit to `main`.
4. GitHub Pages redeploys automatically within about a minute.

No servers, tokens, or AWS resources involved — this is a plain static site.
