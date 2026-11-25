---
name: premium-editorial-design
description: >
  Design landing pages and marketing sites that look like a $10k+ studio did them, not like AI slop.
  The combined best of three sources (ai-slop-to-premium-hero, editorial-luxury-web-design,
  premium-editorial-design): detects and removes 32 common AI design tells (visual, structural,
  typographic, motion, copy, and page-architecture clichés), then rebuilds with a 6-step premium
  editorial system (monumental type, z-axis depth, physical studio lighting, Swiss grid with 60%
  empty space, liquid glass control dock, one living motion moment), plus a copy system, full-page
  architecture, and a mandatory pre-delivery QA gate. Use whenever building, redesigning, auditing,
  or reviewing a landing page, hero, homepage, product page, portfolio, or marketing site. Triggers
  on "make it premium", "remove AI slop", "make it look expensive", "redesign hero", "audit this
  landing page", or any new landing page build. Also use BEFORE shipping any new landing page or
  hero you generated yourself, as a self-review checklist.
version: 3.0.0
author: Combined from three sources; based on the KOVA ONE audit by @muhammadalim_s
triggers:
  - landing page
  - hero section
  - homepage
  - product page
  - portfolio
  - marketing site
  - redesign UI
  - remove AI slop
  - premium web design
  - editorial design
  - make it premium
  - make it look expensive
  - audit landing page
---

# Premium Editorial Design — Anti AI Slop System

## 0. Provenance and honesty notes (read first)

This skill is the combined best of three sources describing the same method: a ~65-second vertical
design-guide video demonstrating it on a fictional headphone brand called **KOVA** (product:
**KOVA ONE**), a written Editorial Luxury system, and a Premium Editorial system built from the
KOVA ONE audit by @muhammadalim_s. Where the sources disagreed, this file records the resolution
explicitly instead of silently picking one.

- Everything in sections 3 and 5 (the tells, the 6 steps, the numbers like 60% and
  `clamp(6rem, 18vw, 12rem)`) was read directly from the video's on-screen captions and code card.
- The percentages the video quotes ("93% of AI pages", "half of AI sites", "17% of AI pages") are
  the creator's claims, not verified statistics. Use them as rough intuition, never cite them as
  fact.
- The video's audio was not transcribed. Implementation details NOT shown on screen (exact shadow
  values, glass blur radius, easing, font choice for the display face) are marked **[recommended]**
  below and are sensible defaults, not quotes from the video. Adjust them to the brand.
- "KOVA ONE" is only the demo subject. The method is brand-agnostic. Never ship KOVA copy, specs,
  or prices for another brand.
- Tell count: the video and written luxury system list 20 core tells; the premium editorial source
  lists 30 (18 core + 12 extended, merging two core tells and omitting dithered photos). This skill
  keeps the canonical 20 core tells (01–20) and adds the 12 extended tells as 21–32, for 32 total.
  Dithered photos (tell 20) is kept from the video source.

## 0b. Operating rule

Never treat this guide as loose aesthetic advice. Treat Phase 1 as **hard lint errors (zero
tolerance)** and Phase 2 as the **default architectural blueprint** for hero sections and flagship
product pages.

## 1. Core philosophy — read this first

You are not a template generator. You are a senior editorial designer from a high-end studio.

**The core insight from the KOVA ONE audit:** removing AI slop is not enough. A clean page after
removing slop is still forgettable. Premium comes from *deliberate editorial decisions* that
create tension, hierarchy, and restraint.

**The 2-phase rule for every task:**
1. **STRIP:** remove every AI tell until the page is boring but clean.
2. **REBUILD:** add back ONLY the 6 premium moves. Nothing else. If a decision is not in the
   6 moves, do not add it.

**The Premium Test:** if you screenshot the hero and blur the logo, can someone still tell it is
expensive? If not, you failed. Expensive is felt through type scale, space, light, and restraint,
not through badges, glows, or gradients.

**Golden rules:**
- One hero moment. One typeface family for display. One accent action. One motion moment.
  Everything else is quiet.
- If you are tempted to add a decoration, add whitespace instead.
- If you are tempted to add a feature card, add a typographic statement instead.
- If you are tempted to add a badge, delete it.
- Real beats perfect. Real shadows beat glows. Real specs beat fake stats. Real photography beats
  3D blobs.

## 2. When to use this skill

Use when the user asks for:
- A new landing page, homepage, hero, product page, waitlist page, portfolio
- "Make it premium / expensive / high-end / Apple-like / Awwwards-level"
- "Remove AI slop / make it not look AI-generated"
- An audit, critique, or redesign of an existing page
- A hero redesign, pricing section, feature section

Do NOT use this skill for:
- Dashboards, admin panels, SaaS app UI, docs, forms-heavy internal tools. Those need clarity,
  not editorial drama.
- If the user explicitly wants playful, brutalist, Y2K, maximalist style, tell them this system
  will fight that style, then adapt only if they insist.

## 3. Phase 1 — the strip audit: 32 AI tells to delete

Audit the current design or your own first draft against this list. Delete or replace every item.
Do not keep any "just one is okay" exception. The power is in the *absence* of all of them
together. The 20-tell purge applies to the WHOLE page; the 6-step premium recipe applies to the
HERO (and its visual language can be echoed down the page).

### 3.1 Typography tells

### Tell 01: Arrows on every button
*"Arrows on every button: Claude →, GPT ↗"*
- Slop: button/link text ending in `→`, `↗`, `->`, or an arrow icon (`ArrowRight`, `ArrowUpRight`,
  `LucideArrowRight`) inside CTAs. Example: "Order KOVA One →", "Explore specs ↗".
- Why it signals AI: AI adds arrows to make buttons feel actionable; it is the default Claude/GPT
  CTA tic.
- Fix: plain, confident typographic labels ("Pre-order", "Specifications"). **Resolution of the
  sources:** no decorative arrows anywhere; at most ONE arrow in the whole hero, only inside the
  glass dock, only if it carries real meaning. All other links are plain text links with underline
  on hover, no arrow. A functional arrow (external-link indicator, carousel prev/next) is fine.

### Tell 02: Little dots between words (interpuncts)
*"Little dots between words: called interpuncts."*
- Slop: `·` or `•` used as separators in meta lines, e.g. "Titanium · Spatial · 60h Battery ·
  Free Shipping", or "DESIGN · SOUND · COMFORT".
- Why it signals AI: lazy spec stuffing; AI uses dots to fake a spec sheet.
- Fix: write a complete natural sentence, or place specifications into a structured Swiss grid
  with explicit labels and values, or a real list with line breaks / a 1px divider. Never
  dot-separated keyword salad. (The video's replacement: "Milled titanium with 60-hour battery
  and free delivery.")

### Tell 03: Overusing eyebrows
*"Tiny all-caps eyebrows: on 93% of AI pages."*
- Slop: small uppercase, letter-spaced, often mono or accent-colored label above headings
  ("HOW IT WORKS", "INTRODUCING", "FEATURES", "TESTIMONIALS") repeated on every section.
- Why it signals AI: AI uses eyebrows as scaffolding because it cannot create hierarchy with type
  alone.
- Fix: delete 90% of eyebrows. Keep at most ONE on the entire page, and only if it carries real
  information the heading lacks (e.g. "KOVA ONE / 2026"). Hierarchy must come from size and
  position, not labels. Exception: functional data labels (a spec's name beside its value, see
  step 4) are fine because they carry information. Step 4 also allows one ultra-subtle,
  wide-tracked micro-caption centred above the monumental headline, rendered as quiet grid
  typography, never in a pill or badge.

### Tell 04: Cream backgrounds
*"Warm beige backgrounds: often #F4F1EA."*
- Slop: page/section backgrounds in the warm off-white family (`#F4F1EA`, `#FAF7F2`, `#F5F0E8`,
  `#FAF8F5`, `#F5F1E8`) used as a shortcut to fake editorial warmth. The AI "warm minimal"
  starter kit.
- Fix: pick a deliberate surface. Intentional, high-contrast surfaces: deep obsidian/studio matte
  black (`#050507`–`#0A0A0C`) for dramatic hardware/editorial depth, or crisp pure architectural
  white (`#FFFFFF` / `#F8F8F8`) with razor-sharp ink contrast. For a light-mode brand that
  genuinely needs a light canvas, use cool paper white (`#F7F7F8`) or pure gallery white, never
  warm AI cream. **Brand exception:** a brand's own real palette colour is not the tell — the
  tell is the *default* beige. If the brand's identity genuinely is a warm cream, keep it only
  as a deliberate, named brand token paired with the rest of the brand system, and make the hero
  itself a deliberate contrasting stage (see step 3). Warmth comes from photography and light,
  not background tint.

### Tell 05: One italic emotional word in the headline
*"One emotional italic word: on half of AI sites."*
- Slop: headline with a single word in italic serif for emphasis, e.g. "Sound worth *feeling*
  every day.", "Sound that feels *real*."
- Why it signals AI: every AI template uses this to fake editorial voice.
- Fix: set the whole headline in one style. No italic in headlines, ever. If you need emphasis,
  use scale, weight, line break, or color. Italic is allowed ONLY inside a long-form pull quote,
  never in a hero headline. Create hierarchy through monumental scale, weight, and spacing, not
  single-word styling tricks.

### Tell 06: Sparkle icons
*"Sparkle emojis: even on non-AI buttons."*
- Slop: ✨, sparkle/`Sparkles` icons, 4-point star glyphs, stars, wand icons on buttons, badges,
  or headings — even on non-AI physical products.
- Why it signals AI: literal visual cliché.
- Fix: remove. Strictly banned everywhere unless literally representing a generative AI action
  (and even then, prefer geometric or typographic indicators). No decorative icons: if you need an
  icon, use a 1px line icon, a real product detail, or a typographic symbol like `->`, `+`, `*`.
  Never sparkles. **Brand exception:** a brand's own signature motif (e.g. a gold sparkle that
  is the brand's real Instagram identity) is not this tell — but keep it out of buttons and
  headings, use it at most once as a restrained brand mark, and flag the judgement call in the
  report.

### Tell 07: Everything in a card
*"Every box wrapped in a border: Gemini's favourite."*
- Slop: every stat, feature, quote, and CTA wrapped in a rounded bordered box with padding and
  shadow (`rounded-xl border bg-white p-6`).
- Why it signals AI: cards are the laziest way to group content.
- Fix: remove containers. Use the page itself as the container: spacing, alignment, type scale,
  and thin hairlines (1px lines) to group things. In the demo, stats became bare numbers with a
  small caption and features became plain text columns. Cards are allowed ONLY for the one
  interactive control (the glass dock) or a true product card in a shop grid. Features are NOT
  cards. They are type + rule + space.

### Tell 08: The word "quiet" (and poetic LLM filler)
*"The word 'quiet': Claude loves it."*
- Slop: grep copy for `quiet`, `quietly`, `quietest` ("Engineered for your quiet mornings...",
  "Quiet luxury"), plus the wider family: `elevate`, `unlock`, `seamless`, `cutting-edge`,
  `next-level`, `revolutionary`, `immersive`, `transform`, `supercharge`, `game-changer`,
  `delve`, `tapestry`, `landscape` (as metaphor), `leverage`, `empower`, `ultimate`,
  `crafted`, `reimagined`, `bespoke`, `unleash`, `truly`, `effortless`, `discover` / `explore`
  (as CTAs), and `premium` in user-facing copy (internal label only, never in a headline).
  The word "real" is its own tell — see tell 16. The full banned-words list lives in section 4.
- Why it signals AI: AI uses these words to fake taste and emphasis while saying nothing.
- Fix: strip pretentious AI poetry. Delete or replace with the specific, verifiable fact the
  filler was pretending to supply ("Hand-matched 40mm beryllium drivers, calibrated individually
  in Zurich."). Applies to YOU as well: when generating copy, avoid these words as default
  adjectives. (The video itself uses "quiet" ironically in a caption; do not treat that as
  permission.)

### Tell 09: Numbered sections
*"01, 02, 03 sections: on 17% of AI pages."*
- Slop: "01 / 02 / 03" counters on feature items or section headers (demo had orange 01 02 03
  above features), or "01 - Design, 02 - Sound, 03 - Battery" with big ghost numbers.
- Why it signals AI: fake editorial structure.
- Fix: remove the numbers. Order is implied by layout and real typographic hierarchy. Use numbers
  only when the sequence is the content (genuine steps in a process, e.g. a chronological setup
  workflow) or as real spec data (e.g. "40h", "32 Ohm"), never as decoration.

### Tell 10: Pulsing green dots
*"Pulsing green dots: every page is 'live'."*
- Slop: small green circle with a CSS pulse animation (`animate-ping`, `animate-pulse`,
  `@keyframes pulse`) next to text like "Shipping live from Zurich", "Now live", "Available",
  "LIVE", "IN STOCK", "2,341 PEOPLE VIEWING".
- Why it signals AI: fake urgency; every page is "live".
- Fix: delete the dot and the fake "live" status. Banned for marketing statements. Only use
  status indicators for genuine real-time telemetry (server health, live audio streams, active
  WebSocket state). If stock is real, state it as plain text in the dock: "In stock". No pulse,
  no dot, no animation.

### 3.2 Layout & structural tells

### Tell 11: Blurry gradient glows behind the hero
*"Blurry gradient orbs: light with no source."*
- Slop: large blurred radial/conic gradients, pink-peach-lavender blobs, purple/blue/orange radial
  blur `filter: blur(80px+)` circles behind the hero.
- Why it signals AI: fake depth without real lighting.
- Fix: remove. Delete all glows. Any light in the final design must have a direction and a source
  (see step 3, studio light).

### Tell 12: Instrument Serif and generic "premium serif"
*"Instrument Serif: AI's go-to display font."*
- Slop: `Instrument Serif`, `Playfair Display`, or any trendy serif as the default "premium" font
  because AI suggested it. It has become the uniform of AI templates in 2025–2026.
- Fix: replace the display face. **Banned by default.** Select a purposeful, characterful
  grotesque, neo-grotesque, geometric sans, or Swiss technical face (e.g. `Neue Haas Grotesk`,
  `Inter Tight`, `Satoshi`, `PP Neue Montreal`, `Space Grotesk` / `Syne` used carefully, `Archivo`,
  `General Sans`, `Helvetica Now` style, or `Helvetica Neue` / `IBM Plex Mono` for technical
  metadata). The demo moved to a heavy modern grotesque sans for the hero title. Never pair serif
  headline + sans body as a default. If you must use serif, use it for ONE small detail like a
  footnote or caption, never the hero. **Brand exception:** a brand's real display serif (e.g.
  Fraunces) is not Instrument Serif — it may stay for editorial subheads, but the monumental hero
  title itself uses the heavy grotesque.

### Tell 13: Colored left borders
*"Thick left bars on quotes: Claude's callout look."*
- Slop: `border-left: 3-4px solid <accent>` / `border-l-4` on blockquotes, callouts, notes, often
  with a light background (e.g. 4px purple/blue left border).
- Why it signals AI: the classic LLM callout/blockquote artifact.
- Fix: plain, well-set quote with attribution, styled via generous margin indentation, refined
  typography, subtle scale shifts, and clean attribution — no thick coloured vertical bars. Quotes
  get huge type, no border, no background, lots of space — or a thin 1px top rule in black/neutral.
  Demo result: the quote in bold text, then "Soren Lindqvist, Mastering Engineer, Stockholm" with
  no bar and no box.

### Tell 14: Three icon cards in a row
*"Three icon cards in a row: the biggest tell."*
- Slop: a row of exactly three equal cards, each with a small icon in a tinted rounded square, a
  title, and 1-2 lines (demo: "Ultra-low latency", "Adaptive seal", "All-day power"). The most
  copied AI layout in existence.
- Fix: remove the cards and icons. Break the row and break symmetry: 1 large statement + 1 image
  + 2 specs pinned to grid corners; or a list with hairlines and large numbers; or one huge
  feature with full-bleed image; or plain text columns; or a single large image with a short stat
  overlay. Never 3 equal columns with icons. The video replaced the trio with plain text columns
  (Beryllium drivers / Milled titanium / Memory seal) plus a large dark image block with one
  concrete figure ("Machined to 0.02mm tolerance.").

### Tell 15: Pills above the headline
*"Badge pills up top: 'New' or 'v2.4'."*
- Slop: small rounded badge above the H1: "New", "v2.4 · Spatial Audio is here", "Now in beta",
  "NOW SHIPPING", "AI POWERED".
- Why it signals AI: AI thinks badges = credibility.
- Fix: remove. Delete all pills. The headline starts the hero; the eye hits the monumental
  typography and subject immediately. If something is truly new, say it in the headline or in the
  dock as plain text (e.g. "Pre-order / Ships March" in the glass dock, not a pill).

### Tell 16: The word "real" as filler
*"The word 'real': doing zero work."*
- Slop: grep `\breal\b` in copy ("Built with real acoustics for real listeners", "Real people,
  real results", "Real sound").
- Why it signals AI: empty emphasis pretending to supply proof.
- Fix: delete or replace with the specific fact that "real" was pretending to supply. Replace
  empty emphasis with verifiable facts: "Hand-matched 40mm beryllium drivers, calibrated
  individually in Zurich."

### Tell 17: Made-up stats
*"99.9% and 12M+: never measured."*
- Slop: round, impressive, unsourced numbers (99.9%, 4.9★, 12M+, "10x faster", "99.9% Noise
  Cancelling", "12M+ Happy Users", "10x Better") with generic captions ("Acoustic purity",
  "Listener rating", "Hours streamed").
- Why it signals AI: numbers without source = lie.
- Fix: replace with real, checkable specifications about the product. The demo used 40mm
  (driver), 248g (Grade-5 titanium), 5-40kHz (measured sweep). KOVA examples: "40h battery",
  "32 Ohm", "254g", "USB-C / 3.5mm". If you do not have a real number, write a sentence instead
  of inventing a stat. Never "12M+".
- **Hard rule for agents: never invent statistics, testimonials, review scores, user counts, or
  named people with titles.** If the user supplied no real data, use obvious placeholders marked
  `TODO: replace with real figure` (or `[NEEDS REAL DATA]`) and tell the user. (The demo's
  testimonial is fictional; do not copy it into real work.)

### Tell 18: Two-word sentences
*"'Pure sound. Every moment.': GPT's favourite."*
- Slop: staccato fragment pairs/triples as headlines and subheads ("Pure sound. Every moment.",
  "Built different. Built to last.", "Built different. Sounds better.", "Quiet power. Loud
  impact.").
- Why it signals AI: AI loves staccato fragments to sound punchy.
- Fix: write one full, confident sentence stating a fact or promise, with a clear subject and
  predicate. Demo: "Tuned flat in Zurich so nothing colors your mix." with supporting line
  "Hand-matched 40mm beryllium drivers, calibrated individually in Zurich." KOVA example: "KOVA
  ONE is a headphone built for long listening, not loud first impressions." One strong sentence
  beats five fragments.

### Tell 19: Sections fading in on scroll
*"Slide up, fade in, repeat everywhere."*
- Slop: every section/card wrapped in an intersection-observer or library (AOS, `whileInView`,
  `IntersectionObserver`) that does `opacity 0 → 1` + `translateY(20-40px)` — e.g. framer-motion
  `initial={{ opacity: 0, y: 24 }} whileInView={{ opacity: 1, y: 0 }}` on every div down the page.
- Why it signals AI: motion as decoration.
- Fix: remove the blanket scroll-reveal. Keep scroll content immediately stable and readable.
  Content appears, it does not perform. Motion budget is spent on ONE hero moment (step 6). Do
  not add scroll-triggered fade-ups to sections below the fold.

### Tell 20: Dithered photos
*"Dithering photos: fake-crafted dots."*
- Slop: halftone/dither/pixel-noise / Floyd-Steinberg filters on imagery used as faux-craft
  texture.
- Why it signals AI: a trendy filter applied to fake "crafted" texture.
- Fix: use clean, high-quality photography or a clean render. Demo replaced the dithered image
  with a crisp dark macro product photo with a short caption. Render crisp, full-resolution,
  cleanly lit photography or transparent PNG/WebP studio cutouts without artificial retro-filter
  gimmicks.

> Milestone in the video: after tell 10 the page "still looks like ChatGPT". Half the list is not
> enough. Keep going.

### 3.3 Extended audit — tells 21–32 (from the premium editorial source)

### Tell 21: Center-aligned everything
- Slop: every section centered, headline centered, paragraph centered, button centered.
- Why it signals AI: centering is the default when there is no grid discipline.
- Fix: default to left-aligned on a grid. Center ONLY the monumental hero word, and only if it
  is edge-to-edge. Everything else aligns to the grid.

### Tell 22: Gradient text / gradient buttons
- Slop: purple-to-blue gradient on headline or CTA.
- Why it signals AI: colored gradient type is a template shortcut for "premium".
- Fix: solid colors only. Black on white, or white on black. Gradient is allowed ONLY inside
  product photography, never in UI text. **Single exception (resolution of the sources):** the
  subtle monochromatic metallic fill on the monumental display word on a dark stage
  (white → light grey, e.g. `#FFFFFF` → `#A1A1AA`) is allowed — it reads as light on metal, not
  as a colored gradient. On light themes the title is solid ink, no gradient.

### Tell 23: Rounded-2xl + shadow on everything
- Slop: every image and card has `rounded-2xl` and soft shadow.
- Why it signals AI: soft rounding + soft shadow everywhere is the AI default finish.
- Fix: images are sharp corners or 2px radius max. One real shadow only on the product cutout
  (see step 3). No border on images, no filters.

### Tell 24: Emoji in headlines / features
- Slop: "🔊 Immersive Sound" — emoji as decoration in UI copy.
- Why it signals AI: emoji replace real iconography and real copy.
- Fix: no emojis in UI. Ever.

### Tell 25: "Trusted By" logo wall of fake companies
- Slop: row of grey logos (Google, Apple, Forbes, etc.) without permission or real coverage.
- Why it signals AI: borrowed credibility with no source.
- Fix: delete unless you have real press. Replace with one real quote in huge type.

### Tell 26: Over-explaining with subheadings under every headline
- Slop: headline + 3-line explanation + bullet list under every section.
- Why it signals AI: the page does not trust its own headline.
- Fix: the headline IS the explanation. Add one line max, or none. Let image and space do the
  work.

### Tell 27: Stock 3D blobs / abstract shapes
- Slop: floating 3D spheres, abstract gradient shapes in hero.
- Why it signals AI: decoration standing in for a real product.
- Fix: use real product photography. One product, shot well, beats any abstract render. If there
  is no product image, use monumental type + a full-bleed lifestyle photo with type overlaid, or
  a pure typographic hero with 60% empty space. Do not use a 3D blob placeholder.

### Tell 28: Sticky nav with blurry background + logo + 5 links + CTA
- Slop: standard SaaS nav — sticky, blurred background, logo, 5 links, CTA button.
- Why it signals AI: the default SaaS chrome, copied everywhere.
- Fix: nav is minimal — wordmark left (16–18px bold, no logo icon needed), 2–3 text links right
  (14px), no background, no border, no CTA. Height 64px. The dock IS the CTA, not the nav.
  Mobile: wordmark + hamburger opening a full-screen menu with huge type.

### Tell 29: Testimonial cards with stars
- Slop: 3 cards with 5 stars, avatar, name, quote.
- Why it signals AI: the testimonial grid is a template, and the stars are unverified.
- Fix: one testimonial, huge type (56–72px), full width, left-aligned, no stars, no card, no
  avatar. Attribution in 13px grey below: "Name — Publication" or "Name — Early listener".
  Example: "I forgot I was wearing them." in 64px type, with a 1px rule.

### Tell 30: Pricing with 3 tiers + "Most Popular" highlight
- Slop: 3 pricing cards, middle one highlighted with color and a "Most Popular" badge.
- Why it signals AI: the pricing-grid template, with a fake popularity claim.
- Fix: if you must show pricing, show ONE price in the dock. Or a clean table with hairlines.
  Never a "Most Popular" badge.

### Tell 31: Footer with 4 columns of links
- Slop: Product / Company / Resources / Legal with 20 links.
- Why it signals AI: the link farm is template furniture.
- Fix: footer is a giant wordmark (edge-to-edge, ~12vw, grey or black, cropped), 1 line of links
  above it (Specs, Story, Support, Instagram) in 13px, and a bottom line ("© 2026 KOVA" left,
  "Designed in [City]" right). That is it.

### Tell 32: "Get Started" / "Learn More" as primary CTA
- Slop: vague CTA — "Get Started", "Learn More", "Try Free".
- Why it signals AI: the CTA says nothing about what happens next.
- Fix: the CTA must be specific: "Pre-order KOVA ONE — $349", "Book a listen", "Download spec
  sheet", "Add to bag — $349". Never "Get Started".

> Note on numbering: tells 01–20 are the canonical core (video + luxury system). Tells 21–32 are
> the 12 extended tells from the premium editorial source. When reporting, cite tells by number so
> the count stays checkable: "N of 32 tells removed".

### Purge verification
After the purge, grep for these quick signals and confirm zero hits (adapt to the stack):

```bash
# copy tells (core + extended banned words)
grep -rniE "\bquiet(ly)?\b|\breal\b|\belevate\b|\bunlock\b|\bseamless\b|\bcutting-edge\b|\bnext-level\b|\brevolutionary\b|\bimmersive\b|\btransform\b|\bsupercharge\b|\bgame-changer\b|\bdelve\b|\btapestry\b|\bleverage\b|\bempower\b|\bultimate\b|\bcrafted\b|\breimagined\b|\bbespoke\b|\bunleash\b|every moment|✨|sparkle|get started|learn more" src/
# glyph tells in UI strings
grep -rnE "→|↗|·|•" src/ --include=*.{tsx,jsx,vue,svelte,html,astro}
# style tells
grep -rniE "Instrument Serif|Playfair Display|F4F1EA|FAF8F5|FAF7F2|F5F1E8|border-left:\s*[2-6]px|border-l-4|backdrop-filter:\s*blur\(\s*[6-9][0-9]px|filter:\s*blur\(\s*(6|7|8|9)[0-9]px|rounded-2xl" src/
grep -rniE "animate-pulse|animate-ping|@keyframes\s+pulse|AOS|whileInView|IntersectionObserver" src/
```
Review hits manually; some are legitimate (e.g. a functional arrow in a pagination or carousel
control, a `whileInView` used once for the single hero moment, a brand's real cream token, a
brand's real serif for subheads).

## 4. Copy system — write like a studio, not a template

### 4.1 Voice rules
- Confident, short, specific. No hype.
- Present tense. Active voice.
- One idea per section.
- Delete adjectives. Keep nouns and verbs.
- Replace vibes with specifics: materials, dimensions, tolerances, places, measured numbers.
  (Demo: "Machined to 0.02mm tolerance." "Calibrated before it leaves Zurich." "Tuned flat in
  Zurich so nothing colors your mix.")
- One idea per sentence, in full sentences. No fragment stacking.

### 4.2 Banned words list
NEVER use these words anywhere in the UI: quiet, real, elevate, unlock, seamless, cutting-edge,
next-level, revolutionary, immersive, transform, supercharge, game-changer, delve, tapestry,
landscape (as metaphor), leverage, empower, discover (as CTA), explore (as CTA), ultimate,
premium (in copy — internal label only, never in a user-facing headline), crafted, reimagined,
bespoke, unleash, truly, effortless. If you catch yourself writing them, replace with a concrete
fact.

### 4.3 Headline formula
Bad: "Experience Sound Like Never Before"
Good: "Headphones for long listening."
Good: "40 hours. No charging anxiety."
Good: "Built to disappear on your head."

Formula: [Product] + [Concrete Benefit] + [Concrete Proof]
Example: "KOVA ONE — 254g, 40h battery, made for all-day wear."

### 4.4 Spec copy
Always write specs as plain facts, not marketing:
- "254g" not "Featherlight design"
- "40h battery, USB-C" not "All-day battery life"
- "Memory foam, replaceable pads" not "Ultimate comfort"

### 4.5 CTA copy
- Primary: "Pre-order — $349" / "Add to bag — $349"
- Secondary: "See specs" / "Read the story"
- Never: "Get Started", "Learn More", "Try Free" (see tell 32)
- CTA labels are verbs/nouns, plain text: "Pre-order", "Order KOVA One", "Explore specs".

### 4.6 No invented proof
Stats, quotes, logos, review scores must come from the user's real data or be flagged as
placeholders (see tell 17).

## 5. Phase 2 — the 6-step premium rebuild

This is the ONLY rebuild system. Do not invent extra steps. Subject: a product hero (the demo is
a dark, studio-lit product page). The same logic generalizes to any product, but if the brand has
no photographable/renderable hero object, tell the user step 2 needs an alternative focal element.
Progress labels in the video: PREMIUM 01/06 … 06/06.

### Step 1: Monumental type scale
*"Scale one bold typeface edge to edge."* On-screen annotation: **"93% viewport · 162px display"**.
- One bold, heavy sans display word (the product name, "KOVA ONE") set so it spans nearly the full
  viewport width — target ~90–94% of viewport width. This is the hero. Not a headline in a
  container. A monument.
- Style: white-to-silver vertical gradient fill on the text (metallic feel — the single allowed
  gradient, see tell 22), very tight tracking, all caps, near-black background. On light themes
  the title is solid ink, no gradient.
- Scale target: `clamp(80px, 17.5vw, 300px)` (the video's code card uses
  `clamp(6rem, 18vw, 12rem)`; the luxury blueprint uses `clamp(4.5rem, 17vw, 13rem)`). Adjust the
  `vw` multiplier based on character count so the wordmark spans ~92% of the frame cleanly on a
  single line. Use fluid type — it must scale with viewport, not fixed.
- Typography craft: tight tracking `letter-spacing: -0.04em` to `-0.06em`; tight leading
  `line-height: 0.85` to `0.95`; weight `650`–`800` geometric/grotesk sans, uppercase for product
  names, sentence case for statement headlines. Subtle vertical gradient fill on dark surfaces
  (`#FFFFFF` at top fading to `#A1A1AA` at bottom) to catch the overhead studio key light.
- Note: `18vw` hitting ~162px corresponds to the video's ~900px-wide preview. For other titles,
  18vw will NOT automatically hit 93% width. Size by measurement:
  `font-size ≈ 0.93 × viewportWidth / (textWidthAtFontSize1)`, or use a fit-text approach, then
  keep a `clamp()` floor so it never becomes unreadable on phones. **[recommended]**
- Keep it real text in an `<h1>` (not an image) so it stays accessible and SEO-friendly.
  **[recommended]**
- Hierarchy: hero word = 1 element. Sub-headline = 18–20px, max 40 characters, placed in a corner
  or below with lots of space. Never the same size as the hero.
- **Do:** let type bleed off edges; one line only; huge contrast between hero word and body
  (hero 180px, body 16px).
- **Don't:** two lines of huge type; huge type inside a rounded card; huge type with a badge
  above it.
- **QA check:** at 1440px width, hero word should be at least 160px tall. If it is smaller,
  increase. Title spans roughly 90–94% of viewport width at desktop, stays legible on mobile
  (clamp floor).
- Code pattern:
  ```css
  .hero-word {
    font-family: "Inter Tight", "Archivo", sans-serif;
    font-size: clamp(88px, 17.5vw, 300px);
    font-weight: 650;
    letter-spacing: -0.05em;
    line-height: 0.85;
    text-transform: uppercase;
    white-space: nowrap;
    margin: 0;
    padding: 0;
  }
  ```

### Step 2: Image over text — break the Z-axis
*"Float the hero dead center over the headline."* Annotations: **Z:01 display type (behind)**,
**Z:02 hero over text (front)**. Never trap the headline in a left column and a boxed rectangular
photo in a right column (the classic generic 50/50 split). Layer the focal subject directly over
the giant typography to create magazine-cover physical depth.
- **Stacking architecture:**
  - `z-index: 0` — Studio background & directional key light stage.
  - `z-index: 1` — Monumental display typography (`pointer-events: none; user-select: none;`).
  - `z-index: 2` — Centered hero visual (transparent product cutout, 3D canvas, or floating
    framed hardware/UI artifact) overlapping the middle characters of the headline.
  - `z-index: 3` — Swiss grid perimeter metadata, minimal top navigation, and the bottom Liquid
    Glass Control Dock.
- A transparent-background cutout of the product sits dead center and overlaps the giant title, so
  the product covers parts of the letters ("KO[V]A [O]NE" is partially hidden). This depth is the
  single biggest quality jump in the video.
- **Overlap:** product must overlap type by at least 30% of its height. Not floating above, not
  below. OVER. **Scale:** product should be 55–70% of viewport height — big enough to feel
  tangible.
- **Legibility rule:** ensure the first and last letters of the monumental wordmark remain clearly
  readable around the silhouette of the overlapping subject (aim for 25–40% central occlusion max).
- Requirements: the cutout MUST be a clean alpha-channel image (PNG/WebP/AVIF) with a precise
  mask: no halos, no leftover background. If the user has only a photo with a background, run
  background removal first and verify edges on a dark background. **[recommended]**
- Both elements must share a stacking context (same positioned container, `isolation: isolate`).
  Center with grid/flex or absolute centering; keep the product's visual center close to the
  title's center. Use `overflow: hidden` on the hero to allow cropping. **[recommended]**
- **Do:** cutout clean, no background, no glow; product overlaps type, not sits in a box.
- **Don't:** product inside a card, circle, or blob; product with drop-shadow glow; multiple
  products floating.
- Code pattern:
  ```html
  <section class="hero">
    <h1 class="hero-word">KOVA ONE</h1>
    <img src="kova-one-cutout.png" class="hero-product" alt="KOVA ONE headphones" />
    <div class="hero-meta"><!-- specs pinned to corners --></div>
  </section>
  ```
  ```css
  .hero { position: relative; overflow: hidden; height: 92vh; }
  .hero-word { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 1; }
  .hero-product { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -48%); z-index: 2; height: 68vh; }
  ```

### Step 3: Studio light, real shadow
*"One directional key light: real grounded depth."* Annotations: **"KEY LIGHT · 45° OVERHEAD"**,
**"GROUNDED SHADOW"**.
- Replace the fake ambient glow (tell 11) with exactly ONE light source: a soft light from
  above/45°, visible as a gentle falloff on the background behind the product, plus specular
  highlights already in the product image. Light direction: pick ONE — top-left 45 degrees (or
  top-center). Keep consistent across all images.
- Place a single soft radial highlight anchored near top-center (`50% 0%` or `50% 15%`),
  illuminating the upper crown of the subject and subtly falling off into deep matte shadow toward
  the edges. Avoid multi-color rainbow gradients. Keep light neutral/achromatic
  (`rgba(255, 255, 255, 0.08–0.14)`) or tinted subtly by the product's material (e.g. cool
  titanium silver).
- A grounded shadow sits beneath the product. Use a dual-layer shadow directly beneath it:
  1. **Tight contact/core shadow:** small, darker horizontal ellipse directly under the lowest
     point of the object.
  2. **Broad ambient falloff:** wider, heavily blurred soft ellipse grounding the product to the
     stage floor.
- **[recommended]** implementation:
  ```css
  .hero { background:
      radial-gradient(60% 45% at 50% 0%, rgba(255,255,255,.10), transparent 70%),  /* key light from above */
      #05060a; }
  .hero-product {
    filter: drop-shadow(0 32px 32px rgba(0,0,0,0.22))
            drop-shadow(0 8px 12px rgba(0,0,0,0.18));
  }
  .ground-shadow {
    position: absolute; bottom: 12%; left: 50%; transform: translateX(-50%);
    width: 42%; height: 28px;
    background: radial-gradient(ellipse, rgba(0,0,0,0.35) 0%, transparent 70%);
    filter: blur(8px); z-index: 1;
  }
  ```
- Rule: light direction, shadow direction, and highlights must agree. If the product photo is lit
  from the top-left, the shadow falls bottom-right. One light, never several colored glows. One
  shadow direction. Shadow is dark, soft, grounded (under product, not behind). Light is
  consistent.
- **Don't:** colored glows (purple, blue, orange); multiple shadows in different directions;
  `box-shadow: 0 0 80px rgba(128,0,255,0.5)` — instant slop.
- **QA check:** squint at the hero. If you see color fringing or halo, delete it. Shadow should
  be grey/black, not colored.

### Step 4: Swiss grid, 60% empty space
*"Pin real specs to the corners: 60% empty space."* Annotations: **"SWISS GRID · 60% EMPTY SPACE"**.
- Generic AI heroes pack ~82% of the viewport with badges, bullets, stats, and cards (leaving only
  ~18% negative space). Editorial luxury inverts this ratio. Remove everything non-essential.
  **Spatial budget target: ≥60% of the hero viewport must remain uncluttered negative space.**
  If it feels full, remove something. Leave space — if in doubt, add 80px more padding.
- Lock the hero strictly to `min-height: 100svh` (or `height: 100svh; max-height: 1080px` on
  desktop) so the entire composition lands as a single framed poster above the fold.
- Grid: 12-column grid, 24px gutters, 32–48px margins on desktop, 20px on mobile.
- Place four spec blocks pinned to the four-corner grid (demo: lower-left and lower-right pairs),
  each a tiny muted label above a bright value:
  - DRIVER: 40mm Beryllium · MASS: 248g Titanium (left)
  - RESPONSE: 5Hz - 40kHz · ORIGIN: Zurich, Switzerland (right, right-aligned)
  - Or KOVA: top-left "KOVA ONE / 2026", top-right "Headphones", bottom-left "254g / 40h",
    bottom-right "Pre-order".
- Top bar: brand wordmark left ("KOVA"), minimal nav right ("01 · SPECS · STUDIO · BAG (0)" in
  small mono caps). Top-left: clean brand wordmark, crisp weight, zero clutter. Top-right:
  ultra-sparse utility navigation (3–4 links max, uppercase monospace or clean micro-sans).
- Use absolute positioning for corner meta (12–13px, uppercase, tracking 0.08em, muted color).
  Rules: use 1px hairlines (`#E5E5E5` on white, `#222` on black) to separate sections, not boxes.
  Alignment: everything aligns to grid columns. No random centering.
- A faint vertical-line/grid texture on the background is present in the video. **[recommended]**
  keep it extremely subtle (≤ 4-6% opacity).
- The recipe card in the video quantifies it: **"Negative Space: 60%"**, described as "Float hero
  cutout dead center over edge-to-edge display typography." Treat it as a design target: roughly
  60% of the hero's area contains nothing but background.
- Spec values must be REAL for the real product (see tell 17). Use `<dl>`/`<dt>`/`<dd>` semantics.
  **[recommended]**
- Note on tell 03: these tiny all-caps labels are legitimate because they pair with a value; do
  not add decorative eyebrows. Left and right flanks stay completely empty breathing room framing
  the centered hero object.
- Code pattern:
  ```css
  .hero-meta { position: absolute; font-size: 12px; letter-spacing: 0.08em; text-transform: uppercase; color: #666; }
  .meta-tl { top: 24px; left: 32px; }
  .meta-tr { top: 24px; right: 32px; text-align: right; }
  .meta-bl { bottom: 24px; left: 32px; }
  .meta-br { bottom: 24px; right: 32px; text-align: right; }
  ```

### Step 5: Liquid glass control dock
*"One quiet frosted glass dock. Zero clutter."* Annotation: **"1 FROSTED DOCK · 0 CLUTTER"**.
- All commerce controls collapse into one small, pill-shaped frosted-glass bar, bottom center:
  color swatches (2 dots), price (`$590`), and a white pill button "Pre-order" (black text). No
  secondary CTA, no badges, no shipping line. **Zero clutter rule:** no dual-button stacks, no
  trust badges, no sub-CTA disclaimers. It is the ONLY button-like element on the hero. One dock
  per page. Keep it quiet — it should feel like iOS control center, not a banner ad. Hide the
  dock on checkout / thank-you pages.
- **Contents (strict maximum of 3 elements):**
  1. Compact variant/option toggle (e.g. 2 circular material/color swatches or billing toggle).
  2. Clear factual anchor (e.g. price `$890` or tier readout; product name + price).
  3. One high-contrast primary CTA pill button (`Pre-order`, `Start Trial`, `Book Studio`) with
     zero arrows and zero emojis.
- Position: fixed bottom center (`bottom: 24px`, `left: 50%`, `transform: translateX(-50%)`,
  `z-index: 50`) OR absolute bottom-center inside the hero. Choose one, not both.
- **[recommended]** dark-stage glass recipe: `background: rgba(24, 24, 28, 0.55);`
  `backdrop-filter: blur(24px) saturate(160%);` `border: 1px solid rgba(255, 255, 255, 0.12);`
  `box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.18), 0 20px 50px rgba(0, 0, 0, 0.55);`
  The inset top highlight simulates refracted overhead studio light. (The video's code card uses
  `rgba(255,255,255,.06)` + `blur(18px)`; prefer the fuller recipe on dark stages.)
- Light-stage glass recipe: `background: rgba(255,255,255,0.72);`
  `backdrop-filter: blur(20px) saturate(180%);` `border: 1px solid rgba(0,0,0,0.08);`
  `box-shadow: 0 16px 40px rgba(0,0,0,0.12);` with a solid `#0A0A0A` CTA button, white text.
- Code pattern:
  ```html
  <div class="dock">
    <span class="dock-name">KOVA ONE</span>
    <span class="dock-price">$349</span>
    <span class="dock-divider"></span>
    <button class="dock-cta">Pre-order</button>
  </div>
  ```
  ```css
  .dock {
    position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
    display: flex; align-items: center; gap: 16px;
    padding: 8px 8px 8px 20px;
    background: rgba(255,255,255,0.72);
    backdrop-filter: blur(20px) saturate(180%);
    -webkit-backdrop-filter: blur(20px) saturate(180%);
    border: 1px solid rgba(0,0,0,0.08);
    border-radius: 999px;
    box-shadow: 0 16px 40px rgba(0,0,0,0.12);
    z-index: 50;
  }
  .dock-cta {
    background: #0A0A0A; color: #fff; border: none;
    padding: 10px 20px; border-radius: 999px;
    font-size: 14px; font-weight: 600; cursor: pointer;
  }
  ```
- **Do:** one dock per page; keep it quiet.
- **Don't:** two docks, or dock + nav CTA + hero button (pick ONE); glass everywhere — glass is
  for the dock only, not for cards, nav, or sections; neon border on glass.
- Keep a solid-color fallback for browsers without `backdrop-filter`. Keep the CTA label plain
  (no arrow, tell 01). On mobile the dock becomes a full-width bottom bar with safe-area padding.

### Step 6: One living hero moment
*"Save motion for one living hero moment."*
- Exactly ONE piece of motion on the page, on the hero. In the video's frames the product shows a
  slow, subtle vertical float (it drifts a few pixels up and down). The video also uses a
  left-to-right light sweep as its before/after reveal; that sweep is a transition effect of the
  video itself, but a one-time light sweep across the headline on load is a valid hero moment.
- **The signature motion:** a barely perceptible, weightless vertical levitation on the hero
  object (`translateY(0)` to `translateY(-8px)` over `6s`–`8s` with smooth
  `cubic-bezier(0.45, 0.05, 0.55, 0.95)` easing), synchronized with a subtle inverse scale/opacity
  pulse on the grounded floor shadow below it (when the object rises 8px, the shadow softens
  slightly by ~4%). Optionally pair with a slow, understated metallic/specular light sweep, or
  subtle pointer-reactive micro-parallax (`±6px` max, heavily damped). Or: slow rotation of 1–2
  degrees on an 8s loop; or the shadow opacity shifting 0.2 → 0.3 on a 6s loop; or a one-time
  load reveal where the hero word slides up 20px and fades in over 0.8s, ONCE, not on scroll.
  Choose ONE.
- Duration: 5–8 seconds per loop. Slow = premium. Fast = cheap. Easing: `ease-in-out`, never
  `linear` for float, never `bounce`.
- **[recommended]** implementation:
  ```css
  @keyframes breathe {
    0%, 100% { transform: translate(-50%, -48%) translateY(0); }
    50% { transform: translate(-50%, -48%) translateY(-8px); }
  }
  .hero-product { animation: breathe 6s ease-in-out infinite; }
  @media (prefers-reduced-motion: reduce) { .hero-product { animation: none; } }
  ```
- Animate strictly GPU-composited properties (`transform`, `opacity`). Always wrap continuous
  motion in `@media (prefers-reduced-motion: no-preference)` (and provide the `reduce`
  off-switch). Everything else on the page is static. No scroll-triggered reveals (tell 19), no
  hover jiggle, no parallax everywhere, no marquee + float + fade + pulse all at once.
- **Do:** one motion, slow, subtle, almost imperceptible. Motion should feel like the product is
  alive, not like the UI is performing.
- **Don't:** every section animating in; parallax on everything.

## 6. Full page architecture — how to structure a premium landing page

Follow this order. Do not add extra sections unless the user explicitly asks. Total page length:
shorter than you think. If your page is longer than 5 scrolls, you added too much. Cut.

**1. NAV (Minimal)**
- Left: wordmark in 16–18px bold, no logo icon needed.
- Right: 2–3 text links (Specs, Story, Support) in 14px.
- No background, no border, no CTA. Height 64px.
- Mobile: wordmark + hamburger that opens a full-screen menu with huge type.

**2. HERO (Steps 1–6 combined)**
- Full viewport: 92–100vh.
- Monumental type + product over type + studio light + corner meta + glass dock + one living
  moment.
- No badge, no sub-paragraph longer than 1 line, no second button.

**3. STATEMENT (One sentence)**
- Full width, 48–72px, left-aligned, 1 sentence, 120px top/bottom padding.
- Example: "We made KOVA ONE for people who listen for hours, not minutes."
- No card, no icon.

**4. FEATURE — IMAGE + TYPE (not cards)**
- Layout: 7 cols type + 5 cols image, or full-bleed image with type overlaid at bottom-left.
- One feature per block. Max 3 blocks, each with a different layout (alternate left/right or
  full-bleed).
- Each block: large headline (40px) + 2 lines max + 1 spec line.
- Image: sharp corners, no shadow except product cutout.

**5. SPECS — HAIRLINE TABLE**
- Title: "Specs" in 20px, uppercase, tracking.
- Rows: name (left, grey) | value (right, black) | 1px bottom border.
- Example rows: Weight / 254g, Battery / 40h, Driver / 40mm, Charging / USB-C.
- No cards, no icons.

**6. QUOTE — ONE HUGE QUOTE**
- One quote, 56–72px, left-aligned, no stars, no avatar, no card.
- Attribution in 13px grey below: "Name — Publication" or "Name — Early listener".
- 120px padding.

**7. FINAL CTA — REPEAT HERO MINIMAL**
- Center: product name in 72–96px, price below in 16px, ONE button (solid black)
  "Pre-order — $349".
- No background color change, no gradient, no card.
- Same dock can stay visible.

**8. FOOTER — GIANT WORDMARK**
- Giant wordmark at bottom, edge-to-edge, 12vw, grey or black, cropped.
- Above it: 1 line of links (Specs, Story, Support, Instagram) in 13px.
- Bottom line: "© 2026 KOVA" left, "Designed in [City]" right.
- No 4-column link farm.

### Adapting the 6-step system beyond hardware products
- **SaaS / app:** the "cutout" can be a floating UI fragment or device render with transparent
  background; the giant title is the product name or a short claim; the four corner "specs"
  become four real metrics or capabilities with measured figures (`LATENCY: <12ms p99`,
  `RUNTIME: Rust / WASM`, `UPTIME: Multi-region active`, `LICENSE: SOC2 Type II`); the dock
  holds one primary CTA (and optional price/plan toggle). B2B SaaS: hero word becomes the product
  name or one-line value prop, product image becomes a dashboard screenshot with real data (no
  fake stats), dock becomes "Book demo" or "Start trial".
- **Services / agency:** replace the cutout with a single strong photograph or typographic
  object; keep the single-light, grid, and white-space principles.
- **Light-mode editorial:** when the brand demands a light canvas (never warm AI cream
  `#F4F1EA`): surface is architectural cool paper white (`#F7F7F8`) or pure gallery white
  (`#FFFFFF`); monumental type is deep obsidian ink (`#0B0B0D`) with subtle atmospheric light
  falloff; studio light is a soft directional daylight vignette (`rgba(255, 255, 255, 0.9)` crown
  highlight) + realistic crisp soft-gray contact shadow (`rgba(15, 20, 30, 0.16)`); liquid glass
  dock is frosted light glass (`rgba(255, 255, 255, 0.72)` + `backdrop-filter: blur(24px)` +
  `1px solid rgba(0, 0, 0, 0.08)` + solid `#0B0B0D` CTA button).
- **Below-the-fold sections:** never fall back into 3-icon-card grids. Alternate between
  full-bleed editorial imagery with pinned technical captions, wide typographic statements, clean
  specification tables with hairline rules (`1px solid rgba(255,255,255,0.08)`), and asymmetric
  65/35 editorial spreads. Zero scroll-fade fatigue: render below-the-fold typography and specs
  immediately crisp and stable.

## 7. Color, type & spacing tokens

### Color tokens (light theme — default)
```
--bg: #FFFFFF
--bg-subtle: #F4F4F4
--text: #0A0A0A
--text-muted: #6B6B6B
--line: #E5E5E5
--accent: #0A0A0A (accent IS black, not a color)
--dock-bg: rgba(255,255,255,0.72)
--dock-border: rgba(0,0,0,0.08)
```

### Color tokens (dark theme)
```
--bg: #0A0A0A
--bg-subtle: #141414
--text: #FFFFFF
--text-muted: #A0A0A0
--line: #262626
--accent: #FFFFFF
```

**Rule:** no brand color in UI. Brand color lives ONLY in product photography. If you need an
accent for a link, use a black underline, not color.

### Dark-stage reference tokens (from the luxury blueprint)
```css
:root {
  --bg-stage: #060608;
  --ink-primary: #f5f5f7;
  --ink-secondary: rgba(245, 245, 247, 0.52);
  --ink-tertiary: rgba(245, 245, 247, 0.30);
  --glass-bg: rgba(22, 22, 26, 0.58);
  --glass-border: rgba(255, 255, 255, 0.12);
  --glass-specular: rgba(255, 255, 255, 0.18);
  --cta-bg: #f5f5f7;
  --cta-ink: #060608;
  --font-display: "Inter Tight", "Neue Haas Grotesk Display", -apple-system, sans-serif;
  --font-mono: "IBM Plex Mono", "JetBrains Mono", ui-monospace, monospace;
}
```

### Typography tokens
```
--font-display: "Inter Tight", "Archivo", "General Sans", sans-serif
--font-body: "Inter", "Inter Tight", sans-serif
--hero: clamp(88px, 17.5vw, 300px) / 0.85 / -0.05em / 650
--h1: clamp(48px, 6vw, 88px) / 0.95 / -0.03em / 600
--h2: clamp(32px, 4vw, 56px) / 1.0 / -0.02em / 600
--body: 16px / 1.6 / 0em / 400
--caption: 12px / 1.5 / 0.08em / 500 / uppercase
--spec: 13px / 1.5 / 0.04em / 400
```

### Spacing tokens
```
--section-padding: 120px top/bottom on desktop, 64px on mobile
--grid-margin: 32px desktop, 20px mobile
--grid-gutter: 24px
--hairline: 1px solid var(--line)
--radius-image: 2px
--radius-dock: 999px
--radius-button: 999px
```

### Image rules
- Hero product: PNG cutout, transparent, studio lit.
- Lifestyle: real photography, no AI 3D blobs, no stock "happy person with headphones" cliché
  if possible. Use editorial crop, full-bleed.
- No rounded-2xl. No border on images. No filters.

### Reference layout skeleton (dark stage)
Hero is `position: relative; display: grid; grid-template-rows: auto 1fr auto;
min-height: 100svh; padding: clamp(1.25rem, 3vw, 2.5rem); isolation: isolate`. Key light is a
`::before` radial gradient (`ellipse 58% 48% at 50% 6%`, white 0.11 → 0.03 → transparent). The
stage stacks type and subject in one grid cell (`grid-area: 1 / 1`). The footer grid is
`1fr auto 1fr` (left spec cluster, centered dock, right spec cluster). On mobile (≤768px) the
footer becomes two columns with the dock on its own centered row above the specs.

## 8. Coding agent workflow — follow this order

When asked to build or redesign, ALWAYS do this:

**STEP A — AUDIT (if redesign):** list which of the 32 tells are present. Output as a checklist:
```
[ ] Tell 01: Arrows on every button — FOUND in hero
[ ] Tell 07: Everything in cards — FOUND in features
...
```
Do not start coding until the audit is done.

**STEP B — STRIP:** create a clean version with NO tells. No badges, no cards, no glows, no pills,
no fake stats. Show the clean version mentally. Confirm it is boring but clean — and state
explicitly that the cleaned baseline is NOT the finish line.

**STEP C — REBUILD WITH 6 STEPS:** apply steps 1 → 6 in order. Do not skip. If a step does not fit
(e.g. no product image), state what you substituted and why, but keep the principle (e.g. if no
product image, use monumental type + a full-bleed lifestyle image with type overlaid).

**STEP D — COPY REWRITE:** rewrite all copy using section 4 rules. Delete banned words. Replace
fake stats with real specs. If real specs are missing, ASK the user for them. Do not invent.

**STEP E — QA CHECKLIST:** run through section 9 before delivering. Fix every fail.

**STEP F — DELIVER:** deliver code + a short note: "Removed X tells, applied 6 steps: [list]. One
decision I made: [e.g. used black/white theme because...]." List every placeholder you could not
fill with real data so the user can supply them.

## 9. QA checklist — run before you ship

**STOP BEFORE FINISHING.** Before delivering code or replying to the user, run this binary audit
across every generated file (HTML, CSS, JSX/TSX, and copy). If **any** item fails, refactor
immediately before responding. Do not say "it is mostly premium". It is either premium or it is
slop.

**Anti-slop (all 32 must pass):**
- [ ] 01 No button arrows (max one arrow, in the dock only, if functional)
- [ ] 02 No interpunct chains
- [ ] 03 No eyebrow spam (max one, only if it carries real info)
- [ ] 04 No default cream background
- [ ] 05 No single italic word in headlines
- [ ] 06 No sparkles, stars, or emojis as decoration
- [ ] 07 No card wrapping for stats/features/quotes
- [ ] 08 No "quiet" / filler family (`elevate`, `unlock`, `seamless`, `cutting-edge`,
  `next-level`, `revolutionary`, `immersive`, `transform`, `supercharge`, `game-changer`,
  `delve`, `tapestry`, `leverage`, `empower`, `ultimate`, `crafted`, `reimagined`, `bespoke`,
  `unleash`)
- [ ] 09 No `01/02/03` padding
- [ ] 10 No pulsing green dots
- [ ] 11 No blurry gradient blobs
- [ ] 12 No `Instrument Serif` / `Playfair Display` / generic premium serif as display face
- [ ] 13 No thick left borders on quotes/callouts
- [ ] 14 No 3-icon-card row
- [ ] 15 No top H1 pills
- [ ] 16 No filler "real"
- [ ] 17 No made-up stats (99.9%, 4.9★, 12M+); all numbers are concrete, verifiable specs
- [ ] 18 No two-word GPT slogans
- [ ] 19 No scroll-fade spam
- [ ] 20 No dithered photos
- [ ] 21 No center-aligned everything (only the monumental hero word may center)
- [ ] 22 No gradient text/buttons (except the monochromatic metallic fill on the dark-stage
  display word)
- [ ] 23 No rounded-2xl + shadow on everything (images sharp or 2px max)
- [ ] 24 No emojis in UI
- [ ] 25 No fake "Trusted By" logo wall
- [ ] 26 No over-explaining subheadings under every headline
- [ ] 27 No stock 3D blobs / abstract shapes
- [ ] 28 No sticky SaaS nav (minimal nav: wordmark + 2–3 links, no blur/border/CTA)
- [ ] 29 No testimonial cards with stars (one huge quote instead)
- [ ] 30 No 3-tier pricing with "Most Popular"
- [ ] 31 No 4-column footer link farm (giant wordmark + 1 line of links)
- [ ] 32 No vague CTAs ("Get Started", "Learn More")

**Premium rebuild (all 6 must pass):**
- [ ] 01 Monumental type: hero display wordmark scales edge-to-edge (~90–94% viewport width),
  ≥160px tall at 1440px, tight tracking, one typeface family
- [ ] 02 Z-axis overlap: focal hero visual (`z-index: 2`) intentionally overlaps monumental type
  (`z-index: 1`) by ≥30% of its height, first/last letters readable (25–40% central occlusion max)
- [ ] 03 Physical light & shadow: one coherent directional key light + grounded contact/ambient
  shadow, grey/black, not colored
- [ ] 04 Swiss grid (≥60% empty space): real specs pinned to corners; hero is one framed poster
  (`100svh`); generous spacing (120px section padding desktop)
- [ ] 05 Liquid glass control dock: essential controls consolidated into one frosted, hairline-rimmed
  dock (max 3 elements) with zero clutter; the only primary CTA in the hero
- [ ] 06 One living hero moment: motion budget focused into one subtle, GPU-composited hero
  animation (5–8s loop) respecting `prefers-reduced-motion`

**Technical:**
- [ ] Responsive: hero word scales with `clamp()`; dock becomes full-width on mobile; grid
  collapses to 1 col; product ~70% viewport width on mobile; corner meta collapses to 2 lines
- [ ] Accessible: contrast 4.5:1+; alt text on product; focus states; `prefers-reduced-motion`
  respected; title is live text in `<h1>`; decorative layers `aria-hidden`
- [ ] Performance: product PNG/WebP/AVIF optimized and preloaded (LCP element); no huge glow blur
  filters; no heavy JS for scroll animations; layout shift = 0
- [ ] Visual check at 390, 768, 1280, 1920 px widths
- [ ] Fallback when `backdrop-filter` is unsupported
- [ ] No lorem ipsum, no placeholder stats

## 10. Prompts for common tasks

**Task: "Make this landing page premium"**
→ Audit with 32 tells, strip, rebuild with 6 steps, rewrite copy.

**Task: "Build a landing page for [Product]"**
→ Ask for: 1) product name, 2) price, 3) 3 real specs, 4) product image (cutout PNG preferred),
5) one sentence why it exists. If missing, use placeholders but MARK them as `[NEEDS REAL DATA]`
and do not invent fake stats. Then build using section 6 architecture.

**Task: "Redesign hero only"**
→ Do steps 1–6 for the hero only. Do not touch other sections unless asked. Deliver the hero
component in isolation.

**Task: "Make it less AI"**
→ Run audit only. List tells found + one-line fix for each. Do not rebuild unless asked.

**Task: "Give me 3 hero options"**
→ Option A: Monumental Type + Product Over Type (KOVA style)
→ Option B: Full-bleed lifestyle image + Type overlaid bottom-left + Dock
→ Option C: Pure typographic hero — giant statement, no product image, huge whitespace + Dock
All three must pass the QA checklist. Never give 3 variations of the same card layout.

## 11. KOVA ONE — reference example (before / after)

**BEFORE (AI slop):**
- Cream background #FAF7F2
- Pill: "NEW V2.4"
- Headline: "Sound that feels *real*." (italic + banned word)
- Sub: "Pure sound. Every moment. Quiet power."
- 3 icon cards: [Sparkle] Immersive / [Battery] 40h / [Star] 4.9 Rating
- Blurry purple glow behind headphone
- Stats: "99.9% Noise Cancelling · 12M+ Users"
- CTA: "Get Started ->" + "Learn More"
- Sections fading in on scroll

**AFTER (premium):**
- White background #FFFFFF
- No pill, no badge
- Hero: "KOVA ONE" edge-to-edge, 220px, black, -0.05em
- Product cutout overlapping type, studio light, real shadow
- Corners: TL "KOVA ONE / 2026", TR "Headphones", BL "254g / 40h / 40mm", BR "$349"
- Dock: [KOVA ONE — $349] [Pre-order]
- Statement: "Headphones for long listening."
- Specs as hairline table
- One quote in 64px: "I forgot I was wearing them."
- One motion: product breathing 6s loop

**What changed:** not more decoration. Less decoration + bigger type + real light + real space +
one dock + one motion.

## 12. Edge cases & judgment calls

- **No product image?** Use monumental type + full-bleed lifestyle photo with type overlaid. Or
  pure typographic hero with 60% empty space. Do not use a 3D blob placeholder.
- **User wants color?** Color lives in photography, not UI. If they insist, allow ONE muted
  accent for the dock CTA only, and keep everything else black/white. Never gradient.
- **User wants playful?** This system is for premium editorial. If they want playful, keep the
  strip phase (remove slop) but replace steps 1–6 with a playful system. Do not mix playful +
  premium — you get neither.
- **B2B SaaS?** Same system applies, but hero word becomes the product name or one-line value
  prop, product image becomes a dashboard screenshot with real data (no fake stats), dock becomes
  "Book demo" or "Start trial".
- **Mobile first?** Hero word must still be monumental on mobile: clamp ensures it scales.
  Product should be 70% of viewport width. Dock becomes a full-width bottom bar. Corner meta
  collapses to 2 lines, not 4 corners.
- **A brand's real identity conflicts with a tell?** A real brand token is not the tell: a
  brand's own warm cream (kept deliberately, named, paired with the rest of the system), a
  brand's own sparkle motif (at most once, never on buttons/headings), a brand's real display
  serif (subheads only, never the monumental title). Flag the judgement call in the report.
- **No product image and no lifestyle photo?** Pure typographic hero (option C in section 10).

## 13. Final instruction to coding agent

You are not here to be safe. You are here to be decisive.

If a design decision is borderline, choose the more restrained option. Delete before you add.
Make type bigger before you add a graphic. Add space before you add a section. Use one motion
before you add five.

Premium is not what you add. Premium is what you have the discipline to leave out.

When in doubt, re-read the QA checklist. If it fails, it is not premium.

Build it like a studio would. Ship it clean.

## 14. Output format when using this skill

1. If auditing: a table `Tell # | Name | Found? | Location (file:line) | Fix applied`, covering
   all 32 rows.
2. Summarize what was removed (count: "N of 32 tells removed").
3. State explicitly that the cleaned baseline is not the finish line, then describe/implement the
   6 steps.
4. List every placeholder you could not fill with real data (specs, stats, quotes) so the user
   can supply them.
5. Don't mention or reproduce the video's call-to-action; this skill contains only the design
   method.

## 15. Common mistakes to avoid

- **Swapping one tell for another.** Removing the italic serif word and adding a gradient-glow
  badge is not progress. Re-run the audit on your own output.
- **Stopping at "clean".** The video explicitly warns that zero tells is still forgettable. The
  premium steps are required.
- **Overlap without a clean cutout.** Z-axis layering with a rough mask looks worse than no
  layering.
- **Adding more instead of less.** Premium here means ~60% empty space. If in doubt, delete.
- **Multiple motions.** One living moment only.
- **Fabricating specs, stats, or testimonials** to make the page feel complete.
- **Copying KOVA.** Reuse the structure (giant name, centered cutout, four corner specs, glass
  dock), not the brand, copy, or fictional specs.
- **Treating tells as a regex-only problem.** Many tells (flat structure, filler copy) require
  reading the page, not grepping it.
