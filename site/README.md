# dinameyer.com redesign concept

A single-page replacement for the current dinameyer.com. No build step, no WordPress: one HTML file, one image folder.

## Preview

Open `index.html` in a browser, or serve the folder:

```
cd site && python3 -m http.server 8000
```

## Hosting

Any static host works. The simplest options:

- **Netlify Drop**: drag the `site` folder onto app.netlify.com/drop. Live in seconds, free, custom domain supported.
- **GitHub Pages**: push this folder to a repo and enable Pages on it.
- **Vercel / Cloudflare Pages**: point at the folder, no config.

Point the `dinameyer.com` DNS at whichever host she picks when she's ready. The old site stays up until then.

## What to swap in

Everything marked with a small dashed `placeholder` tag on the page is waiting on real content. Remove the `ph` class from the element once it's filled.

| Where | What's needed |
| --- | --- |
| Hero portrait (`assets/dina-hero.jpg`) | A high-resolution original. The current file is a crop from a screenshot of the old site, used only to show the layout. |
| Role cards (Work section) | Optional: a still from each title as a background image. Cards currently use color washes so the layout stands without photos. |
| Appearances | Real event rows: date, event name, city, link to the event page. |
| Ask Dina quote | One answered question from the archive. |
| Contact details | Agent, management, and press contacts. |
| Instagram | The footer Instagram icon has no link yet. Facebook, X, YouTube, IMDb, and Cameo links are set. |
| Privacy and Disclaimer | Link the existing pages or paste their text into new ones. |

## Forms

The two forms (Ask Dina, Contact) show a confirmation but don't send anywhere yet. To make them work without a backend, add a `action` and `method` for a form service such as Formspree, Basin, or Netlify Forms, and remove the inline `onsubmit`.

## Design notes

- Near-black background, warm cream text, brass accent. Cormorant Garamond for headings, Inter for body.
- Sticky navigation with a Cameo call-to-action always visible.
- Fully responsive; mobile menu under 900px.
- Respects `prefers-reduced-motion`.
- No frameworks, no tracking, no cookies.
