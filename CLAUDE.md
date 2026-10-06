# Sevenoaks Church Website

Website for **Sevenoaks Church**, based in Sevenoaks, Kent, UK.

The owner is new to Claude Code: explain things slowly, in plain language, with helpful analogies.

## Brand colours

From the official branding pack. Always use these exact values.

| Name | Hex | RGB | CMYK | Role |
|---|---|---|---|---|
| Teal | `#3c6060` | 60, 96, 96 | 75, 42, 50, 34 | Primary |
| Oat | `#ffeee1` | 255, 238, 225 | 0, 9, 13, 0 | Primary |
| Periwinkle | `#547aff` | 84, 122, 255 | 74, 55, 0, 0 | Secondary |
| Stone | `#a79692` | 167, 150, 146 | 33, 36, 34, 13 | Secondary |
| Mint Blue | `#54fbf4` | 84, 251, 244 | 53, 0, 18, 0 | Accent |
| White | `#ffffff` | 255, 255, 255 | 0, 0, 0, 0 | Neutral |
| Black | `#1a1a1a` | 26, 26, 26 | 76, 67, 61, 83 | Neutral |

Teal and Oat (primary) should dominate the design. Periwinkle and Stone (secondary) support it. Mint Blue (accent) is used sparingly for highlights. White and Black (neutral) are for text and clean backgrounds; use the brand Black `#1a1a1a`, not pure `#000000`.

### Contrast notes (for readable text)

- Teal and Oat pair well in either direction. Use them as the main text/background pairing.
- Mint Blue is an accent only. Use it on Teal (or other dark backgrounds), never on Oat or white.
- White text on Periwinkle is OK for large headings and buttons only, not body text.
- Stone is low contrast. Use it for backgrounds, dividers and small decorative elements, not main text.
- Black text reads well on every brand colour, including Periwinkle and Stone (both pass for body text). Use Black, not White, for body text on those two.

## Typography

From the official branding pack. Follow it exactly and use only these two fonts. Both are free on Google Fonts.

Concept: "A voice with strength and grace". Work Sans gives modern clarity; Josefin Sans adds contrast with tall ascenders and dips below the baseline that echo the movement of tree branches.

### Work Sans (primary typeface)

- Used for **headlines, subheads and body text**.
- Headings: **Medium (500) or Regular (400)** weight, depending on tone and visual balance.
- Body text: **Regular (400)** only.
- Use generous spacing and thoughtful alignment so text feels open, approachable and easy to engage with.

### Josefin Sans (graphical headlines)

- Used **selectively**: graphical headlines or key moments where extra contrast is needed. Not for body text or everyday headings.
- Works especially well **layered over photographic backgrounds**.
- Always use **wide letter spacing**, for breathing room and an elevated, intentional tone.

## Oak grain pattern

A key brand design feature: flowing, wood-grain / contour-style thin lines (like the rings of an oak). Reference: `brand/reference/oak-grain-example.png`.

- Must be **subtle but visible**: background texture, never competing with content.
- Thin, even-weight lines with no fill.
- In the reference, the lines are approx `#bfcac7` on a pale Oat background, which is about **Teal at ~30% opacity**.
- Typically bleeds off the edge of a section or corner, rather than sitting as a contained shape.

## Site brief

Pages wanted:

1. Landing page (home)
2. Welcome
3. Sunday meetings
4. Giving
5. Who we are

Inspiration: UK church sites the owner sees as "culturally on point":

- https://gasstreet.church/
- https://kxc.org.uk/
- https://churchnorth.com/

## How the site is built

Plain HTML and CSS, no build step: open any `.html` file in a browser to view it.

- `index.html`: landing page. Other pages (`welcome.html`, `sundays.html`, `who-we-are.html`, `giving.html`) are linked but not built yet.
- `css/styles.css`: shared styles. Brand colours and fonts are defined once at the top as variables.
- `assets/oak-grain.svg` (Teal lines) and `assets/oak-grain-oat.svg` (Oat lines): the oak grain pattern. Add class `grain grain--top-right` (or `grain--bottom-left`) to a section to use it.
- Sections with a Teal background get class `on-teal`, which flips buttons to Oat and switches the grain to Oat lines.
- Placeholder text the church still needs to confirm is wrapped in `<span class="tbc">`, which is highlighted on screen. Search for `tbc` before going live.
- Each page carries `<meta name="robots" content="noindex, nofollow">` while the site is a draft, to keep it out of search engines. Remove it at launch.
- `brand/inspiration-notes.md`: findings from the inspiration sites and the plan for each page.

## Still to collect from the branding pack

- Logo files
- Tone of voice
- Photography
