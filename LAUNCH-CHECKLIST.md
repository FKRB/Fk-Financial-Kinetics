# FK Financial Kinetics — public-launch gate

Status: **PREVIEW PACKAGE — NOT YET APPROVED FOR PUBLIC RELEASE** (8 October 2026).

## Code / architecture inventory
- Static files: index.html, style.css, script.js, about.html, privacy.html, 404.html.
- User data: browser localStorage `fk-casino-v1` stores virtual chips, XP, game history/ledger, property levels, race history.
- No application backend, login, payments, analytics SDK, external JS/CDN or third-party cookies in bundled files.
- Host access logs and host-supplied scripts must be audited after deployment.
- Casino outcomes use browser random values; client-side data is user-editable and not suitable for trusted leaderboards.

## Must complete before promotion
- [ ] TODO(OWNER): choose operator/public contact and replace placeholders in privacy.html and about.html.
- [ ] TODO(OWNER): confirm target audience/jurisdictions and obtain qualified legal review if needed (especially gaming-themed public content, minors, consumer information, privacy).
- [ ] TODO(OWNER): select static host, inspect host privacy/data practices, confirm TLS/HTTPS and any logging/analytics.
- [ ] TODO(OWNER): verify logo, text, icons, emoji, and any future assets are owned or appropriately licensed.
- [ ] Test Chrome, Safari, Firefox, and iOS/Android in the **deployed** environment.
- [ ] Run keyboard/screen-reader and WCAG-focused accessibility review.
- [ ] Validate game payouts and financial model assumptions against documented independent test cases.
- [ ] Check any added analytics/cookies/storage against current ICO guidance; do not load non-essential tracking before valid consent.
- [ ] Test fresh visitor, existing V3.1 saved profile, reset, disabled storage, corrupted save and long session.
- [ ] Review content for unqualified investment/financial advice claims.
- [ ] Decide whether to remain local-only or build a secure backend for accounts and leaderboards.

## Not yet implemented
- Auth, shared cloud storage, global leaderboards, anti-cheat server validation, contact/support service, age-related controls, payments, formal security audit, legal sign-off.

## Known design constraints
- Data stored on each visitor’s device; no global analytics.
- Finance models are illustrative and not live-market or investment-advice systems.
- Hosting security headers (CSP, HSTS, X-Content-Type-Options, etc.) depend on host and should be assessed there.
