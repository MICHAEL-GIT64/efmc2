# AGENTS.md

## Architecture
- A static single-page site with no framework and no build step. `netlify.toml` publishes `public/`.
- `public/index.html` holds all the markup, CSS (in a `<style>` block), and JS (in a `<script>` block).
- `public/assets/` holds the campaign images (PNG originals).

## Conventions and decisions
- Images are referenced through the Netlify Image CDN (`/.netlify/images?url=/assets/<file>&w=<width>&fm=webp`), never directly, so visitors don't download the full-size PNGs.
- There is no payment backend. Checkout builds a `wa.me` link to the business WhatsApp number `2347059775791` with the cart contents. The cart lives in memory and is lost when the page reloads.
- The same number is used in the footer contact link and the floating WhatsApp button. If it changes, update all three places.
- Product prices are in Naira and formatted with `toLocaleString('en-NG')`.
- Keep the existing dark, red-accented style (CSS variables in `:root`).
