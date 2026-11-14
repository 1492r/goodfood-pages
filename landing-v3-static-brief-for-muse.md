# Landing page v3 — host the exact design as a static page (plan B)

Kit's page editor cannot reproduce the approved design (stat strip and previews shrink, numbered points wrap, headlines inconsistent). Plan B: serve the approved page itself and keep Kit only for the form, the incentive email and the PDF.

## Steps
1. Create a PUBLIC GitHub repository under the same account (suggested name `goodfood-pages`; the main repo is private and GitHub Pages is free only on public repos). Put the contents of `site.zip` at its root (`index.html`, `assets/`, `fonts/`, `README-for-muse.md`).
2. Wire the Kit form: `index.html` has two `<!-- KIT_FORM_EMBED -->` spots (hero and proof band). Follow `README-for-muse.md`: paste Kit's inline HTML embed for form e398230547 in both, keep the `.form` wrapper and `<small>` line, and make the input/button pick up the page's styles (full width, white input, terra button #C2613A).
3. Enable GitHub Pages on the repo (branch main, root). Wait for the URL (https://<account>.github.io/goodfood-pages/).
4. Test from the live page: one signup; the incentive email must arrive with the final PDF (MD5 7a2d5e09a42f7c97734a79588e39f5d1).
5. Return: the live URL, a phone render (390 px) and a desktop render of the live page, and the test-email render. Do NOT change the Kit page itself; it stays as the fallback. Nothing is announced before Sun 15 Nov 12:00 noon ET; the bio link switch happens on the owner's go.
