# dave.dk

A gloriously geeky GeoCities tribute homepage for `dave.dk`, a domain whose only real
job is holding some private email. There's no product here, just a homepage the way the
late 90s and early 2000s made them: a tiled starfield GIF, rainbow WordArt, a scrolling
marquee, an eternal "Under Construction" sign, a fake hit counter, a webring that goes
nowhere, a MIDI jukebox, 88×31 badges, and a hidden nod to the old page's single
`Hello world` link.

The copy and styling stay in character for the era: earnest webmaster voice, a real
repeating background tile instead of CSS gradients, hard bevels instead of soft glows,
no rounded corners, no viewport meta tag (phones get the authentic desktop experience),
and chunky `steps()` animation timing so motion chugs like GIF frames instead of easing
at 60fps. "All your base are belong to us" stays, because that one is timeless.

## What's inside

- **`index.html`**: the entire site. One hand-written file. No frameworks, no build
  step, no dependencies, no trackers. Styling and the 88x31 badges are inline CSS /
  SVG, so the only assets are the GIFs. Opens fine by just double-clicking it.
- **`gifs/`**: authentic animated GIFs salvaged from real 1990s GeoCities pages via the
  Internet Archive's [GifCities](https://gifcities.org/). Hosted locally (not hotlinked)
  so the site stays self-contained and nothing breaks if a source disappears.
  (`stars.gif`, the twinkling background tile, is generated locally in the same chunky
  16-color style.)

## Fun stuff

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
