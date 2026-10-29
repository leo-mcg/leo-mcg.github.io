# Leo-McG — landing page

Static landing page for an independent web design studio, built to be published with **GitHub Pages**. No build step, no dependencies, no trackers.

Contact: **[chiefleo@mail.grokbot.com](mailto:chiefleo@mail.grokbot.com)**

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The page: hero, services, process, work, contact, footer |
| `styles.css` | All styles (palette and fonts are CSS variables at the top) |
| `script.js` | Optional enhancements: scroll reveal, copy-email button, footer year |
| `favicon.svg` | Favicon |
| `og-image.svg` / `og-image.png` | Social share image (source + rendered PNG) |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Run locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

## Publish on GitHub Pages

1. Push this folder to a GitHub repository (branch `main`).
2. In the repo, go to **Settings → Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site appears at `https://<user>.github.io/<repo>/` within a minute or two.

Once the final URL is known, change the `og:image` meta tag in `index.html` to the absolute URL (e.g. `https://<user>.github.io/<repo>/og-image.png`) so link previews pick it up reliably, and optionally add `<meta property="og:url">`.

## Customising

- **Agency name:** "Leo-McG" appears in `index.html` (`<title>`, meta/OG tags, header logo, contact subject line, footer), in `og-image.svg`, and in this README. Search and replace `Leo-McG`; the logo letter is the `L` in `.logo-mark`.
- **Email:** search and replace `chiefleo@mail.grokbot.com`.
- **Colors and fonts:** edit the variables in `:root` at the top of `styles.css`.
- **Work section:** the four "Project slot" cards are CSS placeholders. Replace each `.work-art` contents with an `<img>` (with `alt` text) when real projects are ready.

Motion is subtle and is disabled automatically for visitors who prefer reduced motion.
