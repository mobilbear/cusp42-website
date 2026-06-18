# CUSP42 Labs static website

A lightweight static website for **CUSP42 Labs**, designed for GitHub Pages hosting.

## Positioning

CUSP42 Labs is an independent AI thinking lab and product studio. It builds tools and methods for plural reasoning, scenario analysis, structured disagreement, thought experiments, risk thinking, and long-duration judgment.

## Pages

- `index.html` — brand homepage and core positioning
- `work.html` — current and future projects
- `lab.html` — CUSP42 Thought Lab and methodology roadmap
- `ideas.html` — writing themes and research thesis
- `about.html` — brand meaning, principles, and separation language
- `contact.html` — email and public channel placeholders

## How to host on GitHub Pages

1. Create a new GitHub repository, for example `cusp42-site`.
2. Upload all files in this folder to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save.
6. If using `cusp42.com`, keep the `CNAME` file and configure DNS at the domain registrar:
   - For apex domain: use GitHub Pages A records.
   - For `www`: add a CNAME pointing to your GitHub Pages domain.

## Items to update before public launch

- Replace any remaining placeholder links in `contact.html`.
- Update `sitemap.xml` if you use a different domain.
- Keep CUSP42 links separate from personal publication or employer identity unless you intentionally decide to connect them later.
- If you update the brand visuals, replace `assets/cusp42-hero.jpg`, `assets/cusp42-logo-lockup.png`, and `assets/favicon.png`.

## Brand voice

Calm, credible, builder-oriented, and slightly philosophical. Avoid AI hype language. Emphasize plural reasoning, auditable workflows, AI-based scenario analysis, thought experiments, local-first tools, public-good layer, and long-horizon thinking.


## Consensus Room links included

This version includes public links to:

- Consensus Room product page: https://mobilbear.github.io/consensus-room-site/
- Chrome Web Store install page: https://chromewebstore.google.com/detail/consensus-room-multi-ai-d/emdbnpaicikiaceimoacjlfijgjemebk

They are currently placed on `index.html`, `work.html`, and `contact.html`.

## Visual assets

This version uses the supplied cosmic CUSP/42 hero image and the supplied CUSP42 Labs logo lockup. The header uses the full wordmark logo, while the favicon uses a cropped icon-only version for small sizes.
