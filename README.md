# GEO Content Desk (interactive demo)

A static, no-backend demo. Fictional clients, no login, no API keys. Safe to make public.

Files:
- `index.html`   the whole app (HTML, CSS, JS in one file)
- `og-image.png` 1200x630 preview card for LinkedIn, WhatsApp, Slack, email

## Deploy on Vercel (about 5 minutes)

1. Create a GitHub repo, e.g. `geo-content-desk`, and upload `index.html` and `og-image.png` to the repo root.
2. Go to vercel.com, sign in with GitHub, click Add New > Project, import the repo.
3. Leave every setting on default (Framework Preset: Other, no build command, no output directory). Click Deploy.
4. You get `https://geo-content-desk.vercel.app` (or a similar name if taken). Open it and check it loads.

## Replace the placeholder URL (important)

Link previews need absolute URLs. In `index.html`, replace all 3 occurrences of
`https://YOUR-PROJECT.vercel.app` with your real Vercel URL, then commit.

Mac/Linux terminal:

    sed -i '' 's#https://YOUR-PROJECT.vercel.app#https://YOUR-REAL-URL.vercel.app#g' index.html

(On Linux drop the `''` after `-i`.) Or use find and replace in any editor.

## Check the preview card

- LinkedIn Post Inspector: https://www.linkedin.com/post-inspector/
  Paste your URL and click Inspect. This also clears LinkedIn's cache if you change the image later.

## Indexing

The page ships with `<meta name="robots" content="noindex, nofollow">`, so Google will not list it. Only people with your CV link will find it. Delete that line if you want it searchable.

## On the CV

Use the full URL as a live blue hyperlink with a short label, for example: Live demo: GEO Content Desk.
