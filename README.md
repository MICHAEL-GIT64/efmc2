# EFMC†2 Urban Collective

The online storefront for EFMC†2, a streetwear label. It's a single page with campaign images, the Essentials collection (Signature Tee and Performance Joggers), a shopping bag, and WhatsApp ordering. When a customer checks out, WhatsApp opens with their order summary addressed to +234 705 977 5791.

## Technologies

- Plain HTML, CSS, and JavaScript, with no build step (`public/index.html`)
- Netlify hosting, with the Netlify Image CDN resizing images and serving them as WebP

## Run locally

```bash
netlify dev
```

Open the URL it prints. The image URLs (`/.netlify/images?...`) only load through `netlify dev`. They don't load when the file is opened directly.
