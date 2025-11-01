# Notes-elite

Single-page web app for composing Depot installation notes with Fast-survey visuals.

The UI works fully offline thanks to a service worker. Load an Options.txt once (via the default jsDelivr URL, a pasted value, or a local file) and the selections, notes, and What3Words entry stay cached in your browser.

## Getting started

Serve the static files with any HTTP server:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser.
