# Arcova website

Plain HTML and CSS, no build step, no scripts, no third-party requests. Published to GitHub Pages from the public repo `aswin099/arcova` (copy this folder's contents into it).

| Path | What |
|---|---|
| `index.html` | Arcova home: one card per app |
| `inkly/` | Inkly's page |
| `tuck/` | Tuck's page |
| `hoverbox/` | Hoverbox's page |
| `privacy/` | Inkly's privacy policy (the Google Play link, so keep this path) |
| `site.css` | All styles; app colours are scoped classes like `.t-tuck` |
| `fonts/`, `img/` | Self-hosted fonts (OFL) and images |

## Adding an app

1. Copy `tuck/index.html` to `<app>/index.html` (copy `inkly/index.html` instead for a green, phone-style page).
2. Put the icon in `img/<app>-icon.png`.
3. Add a colour class in `site.css` (copy the `.t-tuck` block and change the variables) and use it on `<body>`.
4. Add a card to the `.apps` grid in `index.html`, above the "More on the way" card, and a link in its footer.
5. If the app collects nothing, say so in its FAQ. If it ever collects anything, give it its own `<app>/privacy/` page first.

Check before publishing: open every page at 390 px wide in light and dark mode, and confirm there's no sideways scrolling and no broken images.
