# Premium Editorial Design — Anti AI Slop System

Design landing pages and marketing sites that look like a **$10k+ studio** did them, not like AI slop.

This is a skill (a reusable instruction file) for AI coding agents. It detects and removes **32 common AI design tells**, then rebuilds the hero with a **6-step premium editorial system** — monumental type, z-axis depth, physical studio lighting, a Swiss grid with 60% empty space, a liquid-glass control dock, and one living motion moment.

The core insight: **removing AI slop is not enough.** A clean page after removing slop is still forgettable. Premium comes from deliberate editorial decisions — tension, hierarchy, and restraint.

> **The Premium Test:** screenshot the hero and blur the logo. Can someone still tell it is expensive? If not, you failed. Expensive is felt through type scale, space, light, and restraint — not through badges, glows, or gradients.

## What it covers

**Phase 1 — Strip: 32 AI tells, zero tolerance.** Organised by category:

| Category | Tells |
|---|---|
| Typography | Arrows on every button · interpunct chains · eyebrow spam · cream backgrounds · one italic word · sparkle icons · everything in a card · "quiet" / filler words · numbered sections · pulsing green dots |
| Layout & light | Blurry gradient glows · Instrument Serif / generic premium serif · colored left borders · three icon cards in a row · pills above the headline · dithered photos · made-up stats · two-word sentences · scroll-fade spam |
| Extended audit | Center-aligned everything · gradient text/buttons · rounded-2xl + shadow everywhere · emoji in UI · fake "Trusted By" logo walls · over-explaining subheadings · stock 3D blobs · sticky SaaS nav · testimonial cards with stars · 3-tier pricing with "Most Popular" · 4-column footers · vague "Get Started" CTAs |

**Phase 2 — Rebuild: the 6-step Editorial Luxury System.**
1. **Monumental type** — one heavy grotesque wordmark, ~90–94% of viewport width
2. **Z-axis depth** — the product cutout floats over the type, breaking the flat 2D look
3. **Studio light** — one directional key light + a real grounded shadow, no glows
4. **Swiss grid** — real specs pinned to the corners, ≥60% empty space
5. **Liquid-glass dock** — all controls in one frosted pill: variant, price, one CTA
6. **One living moment** — a single slow, subtle motion; everything else is still

Plus a **copy system** (banned-words list, headline formula, spec/CTA copy rules), a **full-page architecture** (minimal nav → hero → statement → feature → specs table → one huge quote → final CTA → giant-wordmark footer), **color/type/spacing tokens**, a **coding-agent workflow** (audit → strip → rebuild → copy rewrite → QA → deliver), and a **mandatory pre-delivery QA gate** (all 32 tells + all 6 steps must pass, or it is not premium).

## Install

**Muse** — copy the skill into your custom skills:

```bash
git clone https://github.com/Adarsh-Singh07/bury-ai-slop.git
cp -r bury-ai-slop ~/workspace/custom-skills/premium-editorial-design
```

**Claude Code / any agent with skill support** — copy `SKILL.md` into your skills directory (e.g. `~/.claude/skills/premium-editorial-design/SKILL.md`) or point your agent at this repo. The whole system lives in one file: [`SKILL.md`](SKILL.md).

## Use

Ask your agent to:

- **"Make this landing page premium"** — full audit (32 tells), strip, rebuild with the 6 steps, rewrite copy
- **"Build a landing page for [Product]"** — give it the product name, price, 3 real specs, a product cutout image, and one sentence for why it exists
- **"Redesign hero only"** — steps 1–6 for the hero, nothing else touched
- **"Make it less AI"** — audit only: tells found + one-line fix each
- **"Give me 3 hero options"** — monumental type, full-bleed lifestyle, pure typographic

## License

MIT — see [LICENSE](LICENSE).
