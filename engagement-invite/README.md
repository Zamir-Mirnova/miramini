# Zamir & Sarah — Engagement Invitation

A single-page, self-contained animated invitation (tap-to-open envelope, live
countdown, RSVP form). Everything is inlined into `index.html` — no build step,
no dependencies. It is a **static site**.

## Files
- `index.html` — the entire invitation (fonts, images, logic all inlined).
- `preview.png` — the WhatsApp/social link-preview image (924×540).

## Deploy target
Vercel, as a **static site** (framework preset: **Other**, no build command,
output = repo root).

## ⚠️ One required edit after the first deploy
The social-preview tags at the top of `index.html` contain the placeholder
`__SITE_URL__`. Once Vercel gives the production URL, every `__SITE_URL__` must
be replaced with that URL (no trailing slash), then redeploy — otherwise the
WhatsApp link preview image will not load. Details in the deploy prompt.

## RSVP
The RSVP form posts to a Google Form. It already works and needs no server.
Responses land in the linked Google Form / Sheet.
