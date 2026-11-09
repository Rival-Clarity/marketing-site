# Rival Clarity marketing site

Public marketing website for Rival Clarity, competitor intelligence for founders and small businesses.

**Website:** https://rivalclarity.com/

## Current experience

The homepage describes deployed company research, competitor discovery, pricing/product/messaging monitoring, SEO and Google Ads comparisons, reviews and source ratings, recent X posts, public technology references, saved findings, and the in-app weekly brief. Illustrative companies and evidence are explicitly fictional.

All acquisition calls to action are ordinary links to **https://app.rivalclarity.com/signup**, with existing-account links to **https://app.rivalclarity.com/login**. They work without JavaScript. Account data is collected once in the real Clerk signup flow; no marketing form pretends to save a lead or start monitoring. Account completion requires the visitor to authenticate and verify as directed by Clerk.

The unlaunched $19 plan and mock signup forms have been removed. The original demo entry at `docs/demo/index.html` directs visitors to current features or real account creation. The old demo scripts remain archived in the repository but are not loaded or linked by the public experience.

The November 6 source review found the guided overview, multi-company comparison matrix, private finding review controls, cross-channel brief, and optional weekly email merged at app commit `151a632` but not live. These are clearly marked **Coming next**. Recheck the live application before removing that label.

## Automatic insight illustration

The hero includes an animated, fictional example of watched-page signals becoming a source-backed finding. Pricing, product, and messaging examples cycle through Observe → Connect → Insight. Visitors can pause playback, choose an example with mouse or keyboard (which pauses playback), and inspect its matching sample evidence. The animation pauses outside the viewport and in background tabs, and shows a static insight for visitors who prefer reduced motion. Without JavaScript, the initial pricing example remains readable. The illustration does not run real checks or send requests to data providers.

## Files

- `docs/index.html`, `docs/site.css`, `docs/site.js`: homepage, feature examples, sample brief, FAQs, and live signup links.
- `docs/privacy.html`, `docs/terms.html`, `docs/legal.css`: public policies, last updated November 6, 2026. Contact: legal@rivalclarity.com.
- `docs/demo/index.html`: current destination for old demo URLs.
- `docs/CNAME`: rivalclarity.com.
- `docs/.nojekyll`: serve the static files directly.

## Preview and publish

Run `python3 -m http.server 4174 --bind 127.0.0.1 --directory docs` from the repository root, then open http://127.0.0.1:4174.

GitHub Pages publishes `main:/docs`. Pushing to main updates the existing website. Relative assets support the GitHub Pages project path as well as the custom domain. This repository does not use Sites hosting; preserve GitHub Pages and the configured domain.

Google Fonts supplies Manrope and Inter, with local fallbacks. No analytics or advertising pixels are installed. Conversion effects of the old demo have not been measured; retiring its prominent links is a product judgment, not an established conversion result.
