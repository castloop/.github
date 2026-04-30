# Style guide

Writing rules for every Castloop surface — READMEs, docs, marketing copy, code comments, error messages, commit messages, social posts.

These rules are non-negotiable. Consistency is what makes a brand legible across hundreds of small touch-points.

---

## Brand name

- **Castloop** is one word, capitalized at the start of a sentence, lowercase in body text. Same pattern as Stripe, Linear, GitHub.
- Never shortened. Not "CL", not "loop", not "the cast". Two syllables is short enough.
- Never hyphenated, never split across lines.

## Terminology

- **Runtime** is the noun. "The platform" works for broader pitches.
- **Never call Castloop an "engine".** That word belongs to Unreal Engine and Unity Engine — Castloop sits inside them, not next to them.
- **Characters and directors**, not "agents". Game developers dislike the word "agent" in this context.
- **Living** is the strongest brand adjective: "living characters", "living worlds".
- **Local-first** is preferred over "edge", "offline-first", or "on-device-first".

## Words to avoid

These read as marketing filler and dilute the technical credibility we want with engineering buyers:

- smart, intelligent, powerful, revolutionary, cutting-edge
- AI-powered, AI-driven (when used as filler — fine in specific technical contexts)
- seamless, magical, effortless
- next-generation, world-class, state-of-the-art

Specific differentiators carry the weight: latency numbers, on-device, canon-validated, deterministic replay.

## Casing

- **Sentence case** in all headings, button labels, and titles. Capitalize only the first word and proper nouns.
- **Never** Title Case in headings (no "The Runtime For Living Game Characters").
- **Never** ALL CAPS in body text.

Acceptable Title Case contexts: a person's name, a proper noun (Unreal Engine, Unity, NVIDIA ACE), or a literal product/file name.

## Tone

- Short, declarative sentences. Trust the reader.
- Concrete over abstract. "Sub-200ms first-token latency on Steam Deck" beats "fast on-device performance".
- Honest about state. If something is pre-development, say so.
- No hype, no hedging. State what is and what is not.

## Code comments and error messages

The voice rules above apply here too. In particular:

- Error messages: declarative and specific. `"Canon entity 'mira_riverbend' not found in scope 'crossroads'"` beats `"Canon error"`.
- No marketing language in comments. No "blazingly fast", no "magical".
- Comments should explain *why*, not *what*. The code already tells the reader what.

## Visual identity (brief)

For full visual rules, see the design files in `castloop/homepage` and `castloop/.github/profile`. Quick reference:

- **Charcoal** background `#0F0F10`
- **Off-white** text/mark `#FAFAF7`
- **Warm amber** accent `#E8B14C` — focal dots, links, CTAs
- **Typography**: modern geometric sans-serif (Inter, Söhne, Geist). No serifs. No display fonts.
- **No gradients, drop shadows, glow effects, or 3D treatments.** Flat infrastructure register.

## Tagline

> Castloop — the runtime for living game characters.

This is the canonical tagline. Use verbatim where a tagline fits. Don't rephrase it.
