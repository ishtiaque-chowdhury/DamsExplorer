# Dams Explorer

An interactive explorer of 41,145 dams from Global Dam Watch (GDW) v1.0: a world map, filters, slicers and charts.

Product of the Transboundary Freshwater Diplomacy Database, College of Earth, Ocean, and Atmospheric Sciences, Oregon State University. Additional information about the TFDD can be found at: http://transboundarywaters.science.oregonstate.edu.
https://transboundarywaters.ceoas.oregonstate.edu/spatial-datasets

## Files

- `index.html`: the whole app (page, styles and code).
- `data/gdw_dams.csv`: the dam records (18 columns from the GDW v1.0 barriers table).
- `data/world_boundaries.csv`: simplified country outlines, each tagged with its continent.
- `lib/d3.min.js`: the D3 v7 charting library, included so the site doesn't depend on any other website (ISC licence in `lib/d3-LICENSE.txt`).

## Put it online free with GitHub Pages

1. Create a free account at https://github.com and sign in.
2. Click **+** (top right), then **New repository**. Name it, for example, `dams-explorer`, set it to **Public**, and click **Create repository**.
3. On the new repository page, click **uploading an existing file**. Drag in everything from this folder: `index.html`, `README.md`, and the `data` and `lib` folders. Keep the folder structure. Click **Commit changes**.
4. Go to **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, then click **Save**.
5. After a minute or two, the page shows your address: `https://<your-username>.github.io/dams-explorer/`. Anyone can open it, with no login and no expiry.

To update the site later, upload the changed files to the same repository; the page refreshes within a minute or two.

## Notes

- Opening `index.html` directly from your computer (by double-clicking it) won't load the data, because browsers block reading local files. Use GitHub Pages, or test locally with a small web server, e.g. `python -m http.server` in this folder, then open http://localhost:8000.
- Filters are saved in the page address, e.g. `.../#country=India&uses=Irrigation`, so you can share a link to a filtered view.
- Netlify Drop (https://app.netlify.com/drop) and Cloudflare Pages also host this folder free: drag the folder onto the page.
