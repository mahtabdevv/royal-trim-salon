---
name: The Royal Trim
description: Simple, conventional business site for a men's salon. Near-black ground, one brand gold, Cinzel display over a clean grotesque.
colors:
  bg: "#0e0c09"
  bg-2: "#15120e"
  card: "#1a1611"
  slip: "#1d1812"
  gold: "#d6b25e"
  gold-hi: "#ecd08a"
  gold-ink: "#17120a"
  ink: "#f1ead9"
  ink-2: "#c3b89f"
  ink-3: "#9d927c"
  open: "#7fbf7f"
  shadow: "#000"
  line: "rgba(214,178,94,.16)"
  line-2: "rgba(214,178,94,.32)"
typography:
  display: { family: "Cinzel", weights: [600, 700], use: "h1, h2, brand wordmark" }
  body: { family: "Hanken Grotesk", weights: [400, 500, 600, 700], use: "everything else; prices use tabular-nums" }
  sizes: ["clamp(2.4rem,4.6vw,3.9rem)", "clamp(2rem,4vw,3rem)", "clamp(2.2rem,4.8vw,3.6rem)", "clamp(1.05rem,1.6vw,1.2rem)", "1.08rem", "1.05rem", "1rem", ".95rem", ".92rem", ".9rem", ".88rem", ".85rem", ".82rem"]
rounded: ["8px", "10px", "12px", "14px", "16px", "999px"]
---

# The Royal Trim: design system

The owner asked for a simple, business-style site (reference: a conventional Peshawar salon site). Convention is the commitment: dark ground, brand gold from the logo, clear sections, no decorative concept.

## Colour
- Two-tone brand: near-black grounds (`bg`, alternate sections on `bg-2`) and logo gold (`gold`) for emphasis, prices, primary buttons and icons.
- Text: `ink` for headings and body, `ink-2` for supporting copy, `ink-3` for small notes. All pass AA on both grounds.
- `open` green is used only for the "Open now" status dot.
- Hairlines use `line`; outlined controls use `line-2`.

## Type
- Cinzel 700 for headings, matching the roman capitals on the salon's sign. The second half of a heading is often set in gold (`h2 em`), never italic.
- Hanken Grotesk for body, buttons and price lists; prices are bold gold with tabular figures.

## Layout
- Max width 1180px, gutters clamp(16px, 4vw, 32px). Section padding clamp(72px, 10vw, 120px).
- Section order: sticky header → hero (copy left, photo right with brand badge) → category strip → "Why" four-up grid → Services & prices (tabs) → Gallery (3-up) → Visit (info + map) → FAQ (details) → closing CTA → footer.
- Breakpoints: 980px (single column, panel photo hidden, 2-up grids), 640px (full-width buttons, text nav links hidden).

## Components
- Buttons: `btn-gold` (solid gold, dark text) is the primary action and always books on WhatsApp; `btn-ghost` (1px `line-2` outline) is secondary. Radius 10px, min height 50px.
- Service tabs: pill buttons, selected = solid gold. Panels list services as rows: name (+ sub-line), gold price, and an outlined "Add" toggle (pressed = solid gold, check icon, "Added").
- Booking bar: fixed bottom bar that appears once a service is added; shows count, total and the list, and sends a pre-filled WhatsApp message to +92 320 5733063.
- FAQ: native `details` with a gold chevron.
- Icons: one inline SVG set, solid fill in gold.

## Motion
Only short colour and transform transitions (0.2–0.4s, ease-out). The booking bar slides up. Respects reduced motion.

## Assets
Photos in `img/` are cropped from the salon's printed menu flyers; provenance is embedded in each JPEG. The waxing flyer photo is watermarked stock and is never used. The logo mark is a flat SVG redraw of the sign in `assets/2.webp`.
