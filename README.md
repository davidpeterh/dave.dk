# dave.dk

A gloriously geeky 90s-GeoCities tribute homepage for `dave.dk`, a domain whose only
real job is holding some private email. There's no product here, just vibes: a tiled
starfield, WordArt, a scrolling marquee, an eternal "Under Construction" sign, a fake
hit counter, a webring that goes nowhere, 88×31 badges, and a hidden nod to the old
page's single `Hello world` link.

## What's inside

- **`index.html`**: the entire site. One hand-written file. No frameworks, no build
  step, no dependencies, no trackers. Styling and the 88x31 badges are inline CSS /
  SVG, so the only assets are the GIFs. Opens fine by just double-clicking it.
- **`gifs/`**: authentic animated GIFs salvaged from real 1990s GeoCities pages via the
  Internet Archive's [GifCities](https://gifcities.org/). Hosted locally (not hotlinked)
  so the site stays self-contained and nothing breaks if a source disappears.

## Fun stuff

- Star-GIF cursor trail (the way 90s pages actually did it)
- A localStorage "visitor counter" (client-side theatre, collects nothing)
- A spinning globe, a CAUTION construction sign, and a blinking retro computer
- A webring with exactly one member
- Optional 8-bit chiptune (Web Audio, **off by default**, no autoplay)
- A Konami-code easter egg
- Honors `prefers-reduced-motion` for anyone who wants the disco toned down

## Deploy (Cloudflare Pages, from GitHub)

This is a plain static site — **no build tooling required**.

1. In the Cloudflare dashboard: **Workers & Pages → Create → Pages → Connect to Git**,
   and pick this repository.
2. Build settings:
   - **Framework preset:** `None`
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/`  (the repo root)
3. Deploy. Then add the custom domain under **Pages → your project → Custom domains → `dave.dk`**.

Every push to `main` redeploys automatically.

---

Made with 100% pure HTML, a text editor, and zero frameworks. Best viewed in Netscape
Navigator 4.0 at 800×600. 😉
