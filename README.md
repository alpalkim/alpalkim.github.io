# alpalkim.github.io

Personal website for ALP ALKIM.

## Site Structure

- **Homepage Portfolio**: `/index.html`
  - Modern responsive portfolio layout
  - Animated sections (with `prefers-reduced-motion` support)
  - Featured games section rendered from JSON data
- **Games Data Source**: `/data/games.json`
  - Manage game cards from a single file
- **Support/Contact**: `/support.html`
- **Privacy Policy**:
  - `/scoreblastprivacypolicy.html`
  - `/privacy-policy/word-reveal.html`
  - `/privacy-policy/puzzle-hero-buddies.html`

## Local Development

No build step is required (vanilla HTML/CSS/JS).

Run a local server from the repository root:

```bash
python3 -m http.server 8080
```

Then open: `http://localhost:8080`

> Note: A local server is recommended because homepage game cards are loaded via `fetch('/data/games.json')`.

## Updating Game List

Edit `/data/games.json` and update each game object:

- `title`: Game name
- `description`: Short summary
- `tech`: Array of engine/technology tags
- `image`: Image URL (absolute `https://...` or site-relative `/...`), leave empty for placeholder
- `links`:
  - `play`: Play/Download link
  - `github`: Repository link
  - `itch`: itch.io page
  - `steam`: Steam page

Use empty values (`""`) for unavailable links.

## Deployment

This site is compatible with GitHub Pages (static files, no build required).

For Netlify Forms integration on `/support.html`:

1. Deploy to Netlify (or configure GitHub Pages + Netlify)
2. Netlify detects forms with `data-netlify="true"`
3. Configure email notifications in Netlify dashboard
