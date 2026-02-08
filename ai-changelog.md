# AI Changelog

## 2026-02-08 16:30:00 (Offers & Community Card Grids)

- Converted "What We Offer" (11 items) from bullet list to 3-column card grid with colorful icons and short titles
- Converted "Community & Growth" (2 items) from bullet list to card grid with colorful icons and short titles
- Reuses same `.qualities-grid` / `.quality-card` styles from Qualities section

## 2026-02-08 16:20:00 (Qualities Section Redesign)

- Replaced "Qualities We Care About" bullet list with a 3x2 card grid layout
- Each card has a colorful Lucide icon, short bold title, and description
- Cards: Team Player (blue), Integrity (emerald), Ownership (amber), Communication (violet), Initiative (rose), Efficiency (cyan)
- Responsive: collapses to 2-column at 680px and single-column at 440px

## 2026-02-08 16:10:00 (UI Tweak)

- Changed section header icon color (`--icon-accent`) from orange/red (`#c2410c`) to mint (`#34d399`)

## 2026-02-08 16:00:00 (Security Hardening)

- Added Content Security Policy (CSP) via `<meta>` tag — restricts script, style, font, image, and connect sources to known domains only; blocks framing (clickjacking) via `frame-ancestors 'none'`
- Added Subresource Integrity (SRI) hash (`sha384`) and `crossorigin="anonymous"` to Lucide CDN script to prevent supply-chain tampering
- Changed `rel="noopener"` to `rel="noopener noreferrer"` on both external Typeform links to prevent Referer header leakage
- Created `_headers` file for Netlify with security headers: `X-Frame-Options: DENY`, `X-Content-Type-Options: nosniff`, `Referrer-Policy: strict-origin-when-cross-origin`, `Permissions-Policy`, `Strict-Transport-Security` (HSTS with preload)
- Added GDPR cookie consent banner for Microsoft Clarity — analytics now loads only after explicit user acceptance; preference stored in `localStorage`
- Moved Clarity script from unconditional head load to consent-gated dynamic injection

## 2025-02-08 (Single-page JD site)

- Created `index.html` – single-page job description site for Product Designer role at Exabyting
- Design: clean, minimal layout with embedded CSS; clear typographic hierarchy
- Uses logo from `logos/logo_full_horizontal.svg`
- Content from `docs/Product Designer (Mid-Level) - Exabyting.md`
- Ready for Netlify deployment (static HTML, no build step)
- Added fixed header: logo left, Apply Now button right; button scrolls to #apply section
- Added placeholder CTA below How to Apply bullet points; removed placeholder text
- Added favicon: logos/exa-logomark-default.svg
- Added Microsoft Clarity analytics script (project ID: ve238d1yfm)
- Added Typeform links (https://exabyting.typeform.com/PD) to both Apply CTAs; open in new tab
- Location: added (On-site); Work schedule: Sun–Thu; Requirements: en dash (2–4); How to Apply: portfolio first (required), resume second (optional); removed markup artifacts from source .md
- Typography: line-height 1.7 for body, 1.65 for list items; max-width 65ch for optimal line length; increased paragraph/list/heading spacing; text-wrap: balance on headings; antialiased font rendering
- Added Lucide icons: meta section (map-pin, briefcase, bar-chart-2, calendar, users), section headers (building-2, gift, sparkles, heart, list-checks, check-circle, send), Apply buttons (arrow-right)
