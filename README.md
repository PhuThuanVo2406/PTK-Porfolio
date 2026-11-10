# Omega Sigma · Phi Theta Kappa: legacy site

A single-page legacy site for the Omega Sigma chapter of Phi Theta Kappa at Houston City College – Northwest. It covers the chapter's events, officers, awards, and photo gallery.

- `index.html` is the whole site: plain HTML, CSS, and JS, with no build step. Open it in a browser, or serve the folder with any static host such as GitHub Pages.
- To update the content, edit the `SITE` object near the bottom of `index.html`.
- Photos are in `assets/photos/<event>/`. See [CONTENT.md](CONTENT.md) for the catalog and for how to add events.

To preview locally, run `python3 -m http.server` in this folder and open http://localhost:8000.
