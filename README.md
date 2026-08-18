# Handshake — Account Health & Churn Risk Scorer

CSM-facing prototype for Handshake, a CX-led AI governance tool concept for
a fictional B2B cybersecurity company (Wardenly).

**Live: https://mandlspr.github.io/handshake/**

Single-file static site (`index.html`) — vanilla HTML/CSS/JS, no build step.
Reads account data live from Supabase (read-only, anon key, RLS public SELECT)
and posts escalations to an n8n webhook.

**Demo data only** — all 12 accounts (Moonjar Systems, Velvet Comet,
Cinderloop Labs, Puddleforge, Orbit Nettle, Tallow Metric, Juniper Kite,
Fable Current, Hearth Pixel, Saffron Relay, Moss Meridian, Blue Thimble) are
fictional.

## Local development

Optional — only needed if you're editing `index.html` and want to preview
changes before pushing. Not required to use the tool; use the live URL above
for that.

```bash
python3 -m http.server 8123
```

Then open http://localhost:8123.

## Deploy

Static site, served via GitHub Pages (Settings → Pages → repo root /
`main` branch). Pushing to `main` updates the live URL above.
