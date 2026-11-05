# Rival Clarity marketing site

The marketing website and interactive product mockups for Rival Clarity, competitive intelligence for founders and small businesses.

**Website:** https://rival-clarity.github.io/marketing-site/

## Current status

This is a design prototype. All example companies, account details, findings, and evidence are fictional. Features and the proposed Free Brief and $19/month Founder plans are concepts for review.

Signup, payments, email delivery, and competitor monitoring are demonstrations only. Form entries stay in the browser tab; no accounts are created, no websites are fetched, and no emails are sent. Demo watchlists and saved findings reset on reload.

## Site structure

- `docs/index.html`, `docs/site.css`, `docs/site.js`: the marketing homepage, interactive feature examples, sample brief, pricing, FAQs, and signup concept.
- `docs/privacy.html`, `docs/terms.html`, `docs/legal.css`: public legal pages covering the website, demos, and separate application; linked from the homepage footer and demo signup dialog. Contact: `legal@rivalclarity.com`.
- `docs/demo/`: interactive product mockups with a competitor feed, evidence views, saved findings, watchlist management, email preferences, and sample brief.
- `docs/.nojekyll`: serves these files directly as a static website.

The product demo is linked from the marketing site and is hosted in the same repository. No private preview links, credentials, or hosting-provider configuration are required.

## Preview locally

From the repository root:

```sh
python3 -m http.server 4174 --bind 127.0.0.1 --directory docs
```

Open http://127.0.0.1:4174. The product demo is at http://127.0.0.1:4174/demo/#workspace.

## Publish with GitHub Pages

The repository is public. Pages publishes from the `docs` folder on `main` using **Deploy from a branch**. Pushing changes to that folder on `main` automatically updates the website. No custom build, package installation, or deployment credentials are needed.

All asset and product-demo links are relative, so the site works beneath the `/marketing-site/` project path. A custom domain can be configured later in the repository's Pages settings.

Google Fonts is optional; local fallback fonts are provided. There are no analytics or application integrations in this prototype.

## Legal pages

The Privacy Policy and Terms of Service are effective November 5, 2026. The privacy disclosures distinguish browser-local marketing demos from the separate application at `app.rivalclarity.com`, and describe its current account, monitoring, AI, provider, cookie, and retention behavior. Pricing examples remain proposals. Update these pages when collection practices, providers, retention, or paid-service terms change.
