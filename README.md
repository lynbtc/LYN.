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
## Stack
- Pure HTML/CSS/JS
- No build step
- No dependencies
- Hosted on Netlify
## Typography
- IBM Plex Sans 300 — body
- Inter 400/500/600 — nav, logo
## Colors
| Token | Light mode | Dark mode |
|-------|-----------|-----------|
| background | `#fafafa` | `#1a1a1a` |
| text | `#111111` | `#fafafa` |
## Development
Open any HTML file directly or serve locally:
```bash
python -m http.server 8000
```
## Deployment
Push to GitHub → Netlify auto-deploys.
## License
MIT — see LICENSE
