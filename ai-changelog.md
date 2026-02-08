# AI Changelog

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
