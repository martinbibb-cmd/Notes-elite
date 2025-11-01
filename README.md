# Notes-elite

Single-page web app for composing Depot installation notes with Fast-survey visuals.

The UI works fully offline thanks to a service worker. Load the included Options.md once (via the default jsDelivr URL, a pasted value, or a local file) and the selections, notes, and What3Words entry stay cached in your browser.

## Getting started

Serve the static files with any HTTP server:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser.

## Editing the drill-down survey

All survey sections, checklist items, rule triggers, and what3words behaviour now come from the Markdown file [`Options.md`](./Options.md). The app parses:

* `##` headings → navigation sections.
* Checkbox list items (`- [ ] …`) → selectable tiles.
* Indented bullets without checkboxes → contextual grouping.
* HTML comments such as `<!-- rule: combi_selected = true -->` → automatic arse-cover flags.
* The “Auto Arse-Covers” section → rule-to-disclaimer mappings.

Edit the Markdown, reload the page, and the UI/JSON export will update automatically.
