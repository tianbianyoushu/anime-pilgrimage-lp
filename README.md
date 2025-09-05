# Anime Pilgrimage Japan — Landing Page

Public, bilingual (JA/EN) landing page for anime pilgrimage tours in Japan.

## Contents

- `index.html` — markup, SEO/OG, structured data
- `styles.css` — responsive dark theme
- `script.js` — language switcher, smooth scroll, AJAX booking form

## Booking Form (Formspree)

1) Create a form at Formspree and copy your endpoint ID, e.g. `https://formspree.io/f/abcdwxyz`.
2) Replace the placeholder endpoint in `script.js`:

```js
const FORM_ENDPOINT = 'https://formspree.io/f/your-id';
```

If the request fails (or while the endpoint is placeholder), the form falls back to opening a prefilled Mail app.

## Local Preview

Any static server works:

```bash
python3 -m http.server 5173
# Open http://localhost:5173
```

## GitHub Pages

1) Create a public repo and push these files to the `main` branch.
2) In the repo settings → Pages, set Source: `Deploy from a branch`, Branch: `main` (root).
3) Your site will be live at `https://<user>.github.io/<repo>/`.

## Customize

- Brand and contacts in `index.html` (`APJ`, email, footer)
- Route texts, pricing, capacity
- OG image and logo URLs

