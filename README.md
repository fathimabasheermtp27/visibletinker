# TinkerHub Foundation — website

Static homepage for TinkerHub Foundation (v6, "Illustrated").
No build step: `index.html` is the whole site.

## Run locally
Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000

## Publish on GitHub Pages
Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, folder `/ (root)`.
For a custom domain such as www.tinkerhub.foundation, add it under Settings → Pages → Custom domain
and point a CNAME record at `<your-username>.github.io`.

## Updating content
All programme cards, partner tabs, campus list and documents live in the `Component` script at the
bottom of `index.html` (`renderVals()` and `data()`). Edit the text there; the page re-renders from it.

## Data sources (as of 20 Oct 2026)
- tinkerhubfoundation.frappe.cloud and fundraiser.tinkerhub.org
- TinkerHub member platform (via Metabase): members, active campuses, TinkerSpace check-ins, events, Tink-Her-Hack 3.0/4.0
