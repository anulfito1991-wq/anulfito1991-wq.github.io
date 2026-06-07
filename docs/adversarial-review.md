# Adversarial Review — Acosta Apps hub site

> Red-team critique of `anulfito1991-wq.github.io`, run 2026-06-07, ahead of the Facebook/Reddit promo push.
> Status key: ✅ fixed this pass · 🔜 deferred (needs a decision/asset/account) · 💤 backlog.

## P0 — Credibility & promo blockers
- ✅ **No Open Graph / Twitter cards** — added full OG + Twitter `summary_large_image` meta + a generated 1200×630 share image (`images/og-cover.png`). Shared links on FB/Reddit/iMessage now render a real preview card. *(was the #1 blocker for the promo.)*
- ✅ **Stale hero stat** — "9 Apps Live" → **11**.
- ✅ **Site-wide privacy pointed at one app** (`NeonBlocks/privacy.html`) → new studio-level **`/privacy.html`**; both footer links repointed.
- ✅ **Dead newsletter form** (alert "coming soon") → now a working `mailto:` capture with a Formspree upgrade path commented inline.

## P1 — Conversion / legitimacy
- ✅ **Favicon + apple-touch-icon** — generated gradient "A" mark; wired in `<head>`.
- ✅ **"NEW" ribbons** on the four apps shipped this week (Sober Habit, GLP-1, Tether, CoHalve).
- ✅ **JSON-LD Organization** structured data for rich results.
- ✅ **Hero LCP** — above-the-fold hero images were `loading="lazy"`; switched to `fetchpriority="high"` + `<link rel=preload>`.
- 🔜 **Official "Download on the App Store" badges** — replace text links with Apple's badge asset (licensing-clean asset needed). Currently styled text links.
- 🔜 **Social proof** (★ ratings / review quotes) — needs real numbers pulled from ASC.
- 🔜 **Social links in footer** — needs the real Facebook/TikTok/etc. handles (don't want to guess URLs).
- 🔜 **Privacy-friendly analytics** (Plausible / GoatCounter — not Google) — so the promo push is measurable. Needs an account decision.

## P2 — Polish & scale
- ✅ **robots.txt + sitemap.xml + .nojekyll + 404.html** added.
- 💤 **WebP conversion** — app PNGs are ~1.3 MB total; WebP ≈ −65%.
- 💤 **Category filtering** (Wellness · Games · Productivity) — for when the catalog outgrows a flat scroll.
- 💤 **Custom domain** (`acostaapps.com`) — email already uses it; pointing the site there is a legitimacy upgrade (needs DNS + CNAME).
- 💤 **Copy nits** — hero ends on the weak noun "showcase"; "VA care" appears in the AfterAction blurb (the app was deliberately renamed away from "VA").

## Verified good (don't regress)
- 13/13 images have alt text · `rel="noopener"` on external links · all 11 App Store links resolve live · cohesive dark/light design system.
