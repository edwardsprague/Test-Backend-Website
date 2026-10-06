# Ironheart Advisor Hub — Design Prototype

Static HTML prototype of the Advisor Hub: one place for Ironheart advisors to reach every tool.
Styled to match the Ironheart Commercial theme (dark ink, gold, Cormorant Garamond + Jost).

**This is a design prototype for review, not the production site.** Nothing here is wired to a
back end: forms don't submit, search doesn't search, and the sign-in buttons just link to the hub.

## View it

Open `index.html` in a browser (no build step), or enable **GitHub Pages** on the `main` branch
(root folder) to get a shareable link.

## Pages (click-through order)

| File | Screen |
|---|---|
| `index.html` | Advisor Log In (Google sign-in + email fallback) |
| `hub.html` | Hub home: all tools, grouped |
| `deal-analyzer.html` | Tool 01: pick one of 10 calculators |
| `deal-analyzer-cap-rate.html` | Example calculator page (Cap Rate) |
| `deal-documents.html` | Tool 02: LOI/PSA Builder and Grader |
| `om-tools.html` | Tool 03: Build / Update / Co-Brokerage OM |
| `market-reports.html` | Tool 04: weekly market reports |
| `ask-the-notes.html` | Tool 05: Q&A over class notes (Google Drive) |
| `brokerage-forms.html` | Tool 06: downloadable brokerage forms |
| `needs-board.html` | Tool 07: agents post what clients are looking for |
| `shop-my-closet.html` | Tool 08: brokerage listings (placeholder feed) |
| `crm.html` | Tool 10: CRM "coming soon" page (not linked from the hub) |

Tool 09 (Swag Shop) is a hub card that will link out to the vendor's website; there is no page for it here.

## Placeholders to replace

- Anything in `[brackets]` (form names, class names, advisor names, dates, listing details).
- Swag Shop link (`#` in `hub.html`) needs the vendor URL.
- Header shows "Edward Sprague · Sign out" as a stand-in for the signed-in advisor.
- Tool links for LOI/PSA Builder and Grader (`#`) point nowhere until those pages are designed.

## Design tokens

| Token | Hex | Use |
|---|---|---|
| Ink | `#0d0d0d` | Page background |
| Charcoal | `#1a1a1a` | Alt sections, footer, forms |
| Elevated | `#242424` | Cards |
| Line | `#3a3a3a` | Borders |
| Paper | `#f3f1ea` | Body text |
| Gold | `#c9a96e` | Headings, primary buttons |
| Gold Light | `#e8d5b0` | Sub-headings, hover |
| Gold Muted | `#a0855a` | Eyebrows |
| Gold Deep | `#7a6240` | Borders, numerals |

Gold-filled buttons use ink text only (white on gold fails contrast).

## Notes for reviewers

- Desktop layout (1440px) only. Mobile is not designed yet.
- Styles are inline in each page plus `assets/css/hub.css` (fonts and hover/focus states). For
  production, fold these into the WordPress theme's `theme.json` and `style.css`.
- Intended production login: WordPress accounts with roles, plus Google sign-in, with new
  sign-ins held for approval.

## Assets and licensing

- Fonts: Cormorant Garamond and Jost, SIL Open Font License (see `assets/fonts/OFL-*.txt`).
- Logos: Ironheart Commercial and A.I.R.E. brand assets. Keep this repository **private** unless
  you intend to publish them.
