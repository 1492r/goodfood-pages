# Static landing page (plan B) — how to wire the Kit form

`index.html` is the approved v3 design, pixel for pixel. Two places contain `<!-- KIT_FORM_EMBED ... -->` inside `<div class="form">`: the hero and the proof band.

1. In Kit, open the landing page/form e398230547 → Publish/Embed → take the **HTML** (inline) embed, not the JavaScript one if both exist.
2. Replace the dummy `<input placeholder="Your email"><button>…</button>` lines (keep the `<small>` line) with the embed's `<form>` block. Keep the `.form` wrapper.
3. Style hooks: the page's CSS already targets `.form input` and `.form button`; if Kit's embed uses its own classes, add `class` names or wrap the embed's input/button so they pick up the page styles (full width, white input, terra button `#C2613A`, 14px radius, 17/18px text).
4. Keep the incentive (final PDF) and the incentive email exactly as they are in Kit; nothing changes on the Kit side except that the bio link will point at this page.
5. Test: sign up once from this page; the incentive email must arrive with the final PDF (MD5 7a2d5e09a42f7c97734a79588e39f5d1).
6. Publish via GitHub Pages (public repo, root or /docs). Return the live URL plus a phone render.
