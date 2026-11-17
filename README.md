# CUSP42 Labs static website

A lightweight static website for **CUSP42 Labs**, with production hosting on Cloudflare Pages.

## Positioning

CUSP42 Labs is an independent AI thinking lab and product studio. It builds tools and methods for plural reasoning, scenario analysis, structured disagreement, thought experiments, risk thinking, and long-duration judgment.

## Pages

- `index.html` — brand homepage and core positioning
- Live Civilizational AI Risk Index — https://cari.cusp42.com/
- `moralworld.html` — MoralWorld overview and citation
- `lab.html` — CUSP42 Thought Lab and methodology roadmap
- `atlas.html` — CUSP42 Atlas: curated gateway for AI, institutional risk, political economy, multi-agent reasoning, and scenario analysis
- `atlas.json` — machine-readable companion to the Atlas (resource data for agents and tools)
- `library.html` — research, writing and sources
- `sitemap.html` — navigation and links to the public tools
- `faq.html` — frequently asked questions with FAQPage structured data
- `about.html` — brand meaning, principles, and separation language
- `contact.html` — email and public channel placeholders

### Maintaining the Atlas

The Atlas is designed to be low-maintenance. It favors living sources (research hubs, recurring reports, project homepages, canonical papers) over volatile links. To update it:

1. Edit the resource cards in `atlas.html` (each card carries a "Reviewed YYYY-MM" date).
2. Mirror the change in `atlas.json` and in the ItemList JSON-LD inside `atlas.html`.
3. Update the "Last updated" line in the Atlas hero and `lastmod` in `sitemap.xml`.

An occasional review (once or twice a year) is enough; the resource selection is intentionally durable.

## Deploy on Cloudflare Pages

The production branch is `main`. This static site needs no build command. Use the repository root as the output directory when configuring a Pages Git deployment. For Direct Upload, upload a ZIP with `index.html`, `assets/`, `_headers`, and `_redirects` at its root.

Cloudflare Pages uses `_headers` for response headers and `_redirects` for legacy URLs, including `/cari` and `/cari.html`. The homepage reads the latest available score from the CARI site's public daily JSON feed.

## Brand voice

Calm, credible, builder-oriented, and slightly philosophical. Avoid AI hype language. Emphasize plural reasoning, auditable workflows, AI-based scenario analysis, thought experiments, local-first tools, public-good layer, and long-horizon thinking.


## Consensus Room links included

This version includes public links to:

- Consensus Room web app: https://consensus.cusp42.com/app/
- Consensus Room product page: https://consensus.cusp42.com/
- Chrome Web Store install page: https://chromewebstore.google.com/detail/consensus-room-multi-ai-d/emdbnpaicikiaceimoacjlfijgjemebk

The web app is linked from `index.html` and `lab.html`.

## Visual assets

This version uses the supplied cosmic CUSP/42 hero image and the supplied CUSP42 Labs logo lockup. The header uses the full wordmark logo, while the favicon uses a cropped icon-only version for small sizes.
