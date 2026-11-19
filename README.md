# SCENTÉ — Luxury Fragrance Store

A responsive, single-page storefront built with plain HTML, CSS and JavaScript. It is intentionally framework-free so it can be uploaded directly to an existing GitHub repository and hosted with GitHub Pages.

## Files
- `index.html` — complete website (styles and interactions included)

## Run locally
Open `index.html` in a browser. For a local server, use VS Code Live Server.

## Publish to your existing GitHub repository
1. Open your repository on GitHub.
2. Select **Add file → Upload files**.
3. Upload `index.html` to the repository's root (same level as README.md, not inside another folder).
4. Upload/replace the README if desired, then click **Commit changes**.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select branch `main` (or your default branch) and folder `/ (root)`, then **Save**.
8. Wait for the Pages deployment. The site URL will appear in Settings → Pages.

If the repository already has an `index.html`, GitHub will ask you to replace it. Back up the old file first if you need it.

## Before going live — important edits
- Search in `index.html` for `91XXXXXXXXXX` and replace it with your WhatsApp number including country code, digits only. Example format: `919876543210` (do not include `+`).
- Replace `hello@scente.example` with your real support email.
- Update sample products, prices, fragrance notes and policies to match your real inventory.
- Replace the demo bottle artwork with licensed product photography or real 3D assets when available.

## What works in this static demo
- Responsive luxury storefront and animated CSS bottle artwork with pointer-based 3D tilt.
- Product category filters.
- Add-to-cart, quantity changes, remove item and cart subtotal.
- Wishlist.
- Three-step fragrance finder.
- Customer review submission.
- Local product admin: add/delete products and export catalogue JSON.
- WhatsApp order handoff.

## Important production limitations
This is a front-end prototype, not a secure production commerce backend:
- Cart, wishlist, reviews and admin catalogue are saved in the visitor's browser (`localStorage`) only. They do not sync between devices or customers.
- Admin demo code is `SCENTE2026` and is visible in the page source. It is **not secure authentication**; do not use it to protect real business data.
- WhatsApp ordering is a handoff, not an automated payment or order-management system.
- No payment is collected on the site. To accept real payments, connect a trusted payment gateway (for example Razorpay) through a secure server/backend. Never put secret API keys in this HTML file.
- Real accounts, inventory, order records, secure admin roles, verified reviews, tax/shipping rules and email/SMS notifications require a backend/database.
- Product bottle visuals are CSS illustrations, not photorealistic 3D product models. A true GLB/Three.js model can be added when you have bottle assets.

## Recommended next production step
Keep GitHub Pages for the static frontend, and add a backend such as Supabase/Firebase plus a payment provider integration for real orders and secure admin access.
