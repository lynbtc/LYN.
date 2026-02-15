# lyn.page
Minimal website for LYN — modular saunas, finite by design.
## Pages
| Page | Layout | Description |
|------|--------|-------------|
| `index.html` | centered | Home — logo only |
| `documents.html` | text | Document index |
| `onepager.html` | text | About / thesis |
| `collaborate.html` | text | Partnership info |
| `sauna.html` | split + modal | Product page with module explorer |
| `spa.html` | split | Spa concept |
| `residence.html` | split | Residence concept |
| `productsheet.html` | text | Interactive product sheet with collapsible specs, lightbox, print CSS |
| `invest.html` | text | Growth Credit — password-protected |
| `koerner.html` | text | Manufacturing partner — password-protected |
## Stack
- Pure HTML/CSS/JS
- No build step
- No dependencies
- Hosted on Netlify
## Typography
- IBM Plex Sans 300 — body
- IBM Plex Mono 400 — labels, mono
- Inter 600 — nav, logo
## Colors
| Token | Light mode | Dark mode |
|-------|-----------|-----------|
| `--bg` | `#fafafa` | `#1a1a1a` |
| `--text` | `#1a1a1a` | `#e0e0e0` |
| `--text-muted` | `#a0a0a0` | `#666666` |

Theme persists via `localStorage` (`lyn-theme`). Respects `prefers-color-scheme` on first visit.
## Development
Open any HTML file directly or serve locally:
```bash
python -m http.server 8000
```
## Deployment
Push to GitHub → Netlify auto-deploys.
## License
MIT — see LICENSE
