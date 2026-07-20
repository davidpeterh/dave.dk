# dave.dk

The homepage for `dave.dk`, a domain whose only real job is holding some private email.
Two pages, no trackers, no build step, nothing to buy:

- A calm, modern front door (`index.html`) that just answers "what is this place?"
- A gloriously geeky GeoCities time capsule (`1999.html`), reachable via an easter-egg
  link at the bottom of the modern page.

## What's inside

- **`index.html`**: the modern landing page. Self-contained, theme-aware (light/dark),
  no external requests. An editorial serif paired with a monospace, one warm accent, a
  quiet entrance animation, and a subtle link down to the 1999 edition.
- **`1999.html`**: the full late-90s / early-2000s experience. A tiled starfield GIF,
  rainbow WordArt, a scrolling marquee, an eternal "Under Construction" sign, a fake hit
  counter, a webring that goes nowhere, a MIDI jukebox, 88×31 badges, "All your base are
  belong to us," and a hidden nod to the old page's single `Hello world` link. Styling
  stays in character: real background tiles instead of CSS gradients, hard bevels, no
  rounded corners, and chunky `steps()` animation so motion chugs like GIF frames.
- **`gifs/`**: authentic animated GIFs salvaged from real 1990s GeoCities pages via the
  Internet Archive's [GifCities](https://gifcities.org/). Hosted locally (not hotlinked)
  so the site stays self-contained and nothing breaks if a source disappears.
  (`stars.gif`, the twinkling background tile, is generated locally in the same chunky
  16-color style.)

## Fun stuff (on the 1999 page)

- Star-GIF cursor trail (the way 90s pages actually did it)
- A localStorage "visitor counter" (client-side theatre, collects nothing)
- A spinning globe, a CAUTION construction sign, and a blinking retro computer
- A webring with exactly one member
- An optional 8-bit MIDI jukebox (Web Audio, off by default, no autoplay)
- Honors `prefers-reduced-motion` for anyone who wants the disco toned down

## Deploy (Cloudflare Pages, from GitHub)

This is a plain static site. **No build tooling required.**

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
