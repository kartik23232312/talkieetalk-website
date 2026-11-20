# TalkieeTalk website

Responsive static companion site for the TalkieeTalk mobile app, built with plain HTML, CSS and browser JavaScript. It introduces the app and does not implement authentication, messaging, purchases, voice calling or live rooms.

## Project files

- `index.html` — homepage
- Individual `.html` files — public information pages
- `css/styles.css` — shared brand system and responsive layouts
- `js/site.js` — navigation, footer, FAQ, and contact form behavior
- `js/page-content.js` — content for shared-layout pages
- `assets/` — favicon and social sharing image

## Run locally

No package install or build step is needed. Open `index.html` directly or serve the directory with any static server. For example:

```sh
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Build and deployment

There is no compile step. Deploy the full directory to a static hosting provider, preserving relative paths. Configure HTTPS and a custom domain with the provider, then set DNS as directed by that provider.

The domain `talkieetalk.in` is configured in `CNAME`, canonical URLs, Open Graph metadata, `robots.txt` and `sitemap.xml`. Verify DNS before turning on GitHub Pages HTTPS. Add real app-store links, a verified contact channel and finalized legal documents before launch.

## SEO

All 11 pages have distinct titles and descriptions plus canonical URLs, Open Graph metadata and a Twitter card. The homepage includes basic `WebSite` JSON-LD. `assets/talkieetalk-social.svg` is the share image. After DNS and HTTPS work, submit the sitemap in the search-console account.

## Supabase and authentication

This site intentionally has no Supabase integration and reads no app database. No schema or auth settings were inspected or changed. If website authentication is later required, inspect the existing schema and auth configuration first, use only a publishable/anon browser key, and never put a service-role key in browser code. Do not create or modify tables or policies without review and approval.

## Contact form

The form validates required fields in the browser, then explains that delivery is not configured. It does not claim a message was sent. Connect an approved service or server endpoint before using it as a contact channel.

## Legal review

Privacy Policy and Terms and Conditions are marked as drafts. Add verified organization details and legal review before publication. Premium benefits are described as configurable; no prices or purchase claims are shown.
