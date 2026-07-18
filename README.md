# dave.dk

A gloriously geeky 90s-GeoCities tribute homepage for `dave.dk` — a domain whose only
real job is holding some private email. There's no product here, just vibes: a tiled
starfield, WordArt, a scrolling marquee, an eternal "Under Construction" sign, a fake
hit counter, a webring that goes nowhere, 88×31 badges, and a hidden nod to the old
page's single `Hello world` link.

## What's inside

- **`index.html`** — the entire site. One hand-written file. No frameworks, no build
  step, no dependencies, no trackers. All graphics are CSS / inline SVG / emoji, so the
  page makes **zero network requests**. Opens fine by just double-clicking it.

## Fun stuff

- ✨ Sparkle cursor trail
- 📟 localStorage-based "visitor counter" (client-side theatre — collects nothing)
- 🔗 A webring with exactly one member
- 🔊 Optional 8-bit chiptune (Web Audio, **off by default** — no autoplay)
- 🕹️ A Konami-code easter egg
- ♿ Honors `prefers-reduced-motion` for anyone who wants the disco toned down

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
