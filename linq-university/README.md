# LINQ × University (v5)

One self-contained page: fonts, copy, images and the 3D mask are all inside `index.html`. No build step, no server code, no external calls.

| File | What it does |
|---|---|
| `index.html` | The whole page |
| `netlify.toml` | Tells Netlify to publish this folder as-is, and keeps it out of search engines |
| `robots.txt` | Asks search engines not to index the site |
| `.gitignore` | Keeps Mac and Netlify clutter out of the repo |

## Open it locally
Double-click `index.html`. It works offline in any current browser.

## Put it online (Netlify)
1. **Add new site → Deploy manually**, then drag this folder in.
2. Or from GitHub: create a private repo, upload these files, then **Add new site → Import an existing project → GitHub**. Leave the build command empty; publish directory is `.`.

## Notes
- The page is about 2.0 MB (about 1.4 MB compressed per visit).
- Search engines are asked not to index it. To make it searchable later, remove the `X-Robots-Tag` line in `netlify.toml`, the `robots` meta tag in `index.html`, and `robots.txt`.
- The invitation form opens an email to the contact address in the page. To ship a new version, replace `index.html`.
