# Offline Helper public landing page

This public repository contains only the market-facing static pages for Offline Helper.

The private product/service repository remains separate at `Pdbjork/Offline-Helper`.

## Published pages

- `/` — public landing page
- `/fit-check/` — free fit-check bridge page
- `/confirmed-fit-payment/` — noindex payment handoff page to use only after a confirmed fit check
- `/payment-success/` and `/payment-canceled/` — simple payment state pages

## Privacy and sales guardrails

- Payment stays behind fit check.
- No forms or checkout metadata should ask for passwords, recovery keys, bot tokens, or private documents.
- Messaging should say local-first, not 100% offline, because payments, email, messaging, and support may use cloud services.
- Do not add customer/private pilot notes to this public repo.

## Deployment

GitHub Pages should publish from branch `main`, folder `/`.

Expected staging URL before custom-domain DNS is fixed:

`https://pdbjork.github.io/offline-helper-landing/`

Only add `CNAME` with `offlinehelpers.com` after IONOS DNS points the domain to GitHub Pages and the GitHub Pages site is verified.
