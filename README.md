# preetkaria.com

Personal site. One self-contained `index.html` — no build step, no dependencies.
Fonts load from Google Fonts at runtime; everything else is inline.

## Run locally

Open `index.html` in a browser. That's it.

Or, if you want a local server:

    python3 -m http.server 8000

## Deploy

Vercel auto-detects this as a static site. No framework, no build command,
no output directory. Push to `main` and it ships.

## Editing

Everything lives in `index.html`:

| What | Where to look |
|---|---|
| Colours, fonts, spacing | `:root` at the top of `<style>` |
| Projects (cards + modals) | `const P = [...]` in `<script>` |
| Also-built rail | `const ALSO = [...]` |
| Counters | `const FIG = [...]` |
| Experience / Education / Research tabs | the `.panes` markup |
| Hero name, statement, chips | the `.hleft` markup |

Search for `TODO(preet)` before shipping — those are the gaps only you can fill.
