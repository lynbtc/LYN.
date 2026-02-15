# CLAUDE.md — LYN

## What this is
**LYN** is jsb's operating firm. Bitcoin-native. Accumulates bitcoin through adding value in open markets.

**The sauna project** is LYN's first and current venture. 2,100 numbered outdoor units + unlimited bespoke indoor installations. Designed by Morten Bo Jensen, manufactured by KOERNER Saunabau.

This repo is the live website at lyn.page.

## Deployment — CRITICAL
This repo auto-deploys to Netlify on push to main. **This is a live production site.**

### Rules
1. **Claude Code never pushes or commits.** Only make local file changes.
2. jsb reviews changes locally, commits and pushes to main himself.
3. If unsure about a change, **ask before editing.**
4. Test locally first: `python -m http.server 8000` in repo root.

## Stack
- Pure HTML / CSS / JS
- No frameworks, no build tools, no dependencies
- Google Fonts loaded via CDN (IBM Plex Sans, IBM Plex Mono, Inter)
- Netlify hosting, Cloudflare DNS
- Netlify Forms for submissions (email notification to jsb)

## Pages
| File | Purpose | Notes |
|------|---------|-------|
| index.html | Home — logo only | Centered layout |
| documents.html | Document index | Text layout |
| onepager.html | About / thesis | Text layout |
| collaborate.html | Partnership info | Text layout |
| sauna.html | Product page | Split layout + modal module explorer |
| spa.html | Spa concept | Split layout |
| residence.html | Residence concept | Split layout |
| productsheet.html | Interactive product sheet | Collapsible specs, lightbox, print CSS |
| invest.html | Growth Credit | **Password-protected (lyn2100)** |
| koerner.html | Manufacturing partner | **Password-protected (lyn2100)** |

### Subdomains
- siteplanning.lyn.page — M4 thermal module feasibility configurator (separate repo/deploy)

## Design system
- **Body text:** IBM Plex Sans 300
- **Labels/mono:** IBM Plex Mono 400
- **Logo/nav:** Inter 600
- **Background:** #fafafa
- **Text:** #1a1a1a (or near-black)
- **Layout:** Minimal. No cards, no boxes. Whitespace over borders. Lowercase labels.
- **No emojis, no icons, no decorative elements**

## Copy and code philosophy
Every word earns its place. Every line of code earns its place. If it doesn't add value, cut it.

### Copy
- Factual. No sell lines. No filler.
- Don't explain what the reader should think. State facts, let them connect dots.
- The live lyn.page is the tone reference — match it. When in doubt, read the site.
- Normal capitalization in documents (product sheet, PDF output). Lowercase on website labels.

### Code
- Open-source clean. Readable, minimal, no abstraction for its own sake.
- HTML should read almost like a document. Semantic, obvious structure.
- CSS: as few rules as needed. No utility class sprawl. Whitespace does most of the work.
- JS: only when static HTML can't do it. No libraries unless unavoidable.

## Password gate
Pages using password protection use `lyn2100`. Implementation is inline JS — no server-side auth. The gate hides content until correct password entered.

## Module system
Seven modules: M1 (sauna), M2 (swimming bridge), M3 (changing room), M4 (thermal module), M5 (outdoor shower), M6 (outdoor storage), M7 (cold plunge).

### M4 thermal module
- **Optional.** Not included in every unit.
- At a LYN site, M4 IS the heating system. Electricity = heating cost. Bitcoin = upside.
- Site planning tool evaluates feasibility per site based on thermal demand, electricity cost, climate.
- Positioning: "hard asset for your savings" (not "bitcoin for your savings").

### Stove/heater
- Not fixed to one brand. Curated selection.
- Indoor/commercial → KOERNER stove is default.
- Private outdoor → other stoves in the selection (e.g. HUUM) may be used.
- Specified during design phase based on installation type.

## Working conventions
- Show proposed text copy before implementing in code.
- Deliver code changes as specific find → replace edits unless building a new page.
- Don't rewrite files unnecessarily. Minimal diffs.
- Before starting work on any page, check its current live state — the repo may have changes not reflected in conversation history.
