# A Digital Wilderness

A personal website built as a *digital wilderness* — a wild patch of the internet
that's tended by hand, not tamed into a feed. Inspired by the [digital gardens](https://www.technologyreview.com/2020/09/03/1007716/digital-gardens-let-you-cultivate-your-own-little-bit-of-the-internet/)
idea, but leaning into the wildness: nature front and center, a landscape you
wander rather than a timeline you scroll, and content that's allowed to be
half-grown.

Everything on the site carries a **growth stage**:

- 🌱 **Seed** — just planted, a rough thought
- 🌿 **Sapling** — taking shape, still growing
- 🌳 **Wildwood** — rooted, but never truly finished

## Structure

```
index.html            The whole site (single page, anchored sections)
assets/css/main.css   Styles — palette, type, layout, the hero scene
assets/js/main.js     Mobile nav + footer year (that's it — no framework)
```

No build step, no dependencies. It's plain HTML/CSS/JS so it stays easy to
tend and will host anywhere.

## Run it locally

Just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Any static host works — GitHub Pages, Netlify, Cloudflare Pages, etc.
For **GitHub Pages**: push to your default branch and enable Pages
(Settings → Pages → deploy from branch, root).

## Make it yours — the placeholders to fill in

Search the code for `TODO` and `[Your Name]`. The main spots:

- **Your name & bio** — the "The Tender" section in `index.html`.
- **A real photo of you** — replace the placeholder SVG in "The Tender"
  (something nature-y fits the theme).
- **Your links** — email, newsletter, GitHub, socials (Tender section + footer).
- **Wanderings** — swap the three placeholder essays for your real writing.
- **Field Notes** — your short, living entries; cross-link them freely.
- **Undergrowth** — your projects and experiments.
- **Hero photo** — the hero uses a real nature photograph (a misty-mountain
  "wallpaper" shot) hotlinked from [Unsplash](https://unsplash.com), which is
  free to use. To change the mood, swap the `background-image` URL in
  `.hero__media` (`assets/css/main.css`); a few alternate photo IDs are listed
  in a comment right there. A moody gradient sits behind it as a fallback, so
  the title stays legible even if the image is slow. Prefer to **self-host**?
  Drop a `.jpg` in `assets/img/` and point the URL at `../img/your-photo.jpg`.

## Type & color

- Display face: **Fraunces** (soft, organic, a little "wonky")
- Body face: **Newsreader** (warm and literary)
- Palette: dusk sky, forest ink, warm paper, moss green, ochre accent

## Notes

- Fully responsive, keyboard-accessible, and respects `prefers-reduced-motion`.
- Animations (drifting swallows, swaying grass) are subtle and turn off for
  anyone who's asked their system to reduce motion.
