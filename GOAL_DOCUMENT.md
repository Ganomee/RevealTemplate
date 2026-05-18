# Reveal.js Conference Template Goal Document

## Objective
Create an aesthetically pleasing, moderately animated Reveal.js presentation template for a **conference talk**. The design must align with assets and brand motifs from **easyRadiology** and be delivered as both:

1. a reusable theme system, and
2. a starter deck with sample slides.

## Locked decisions from stakeholder input

- **Use case**: conference talk.
- **Audience**: IT (technical conference audience).
- **Language**: English.
- **Asset source**: use assets from the official easyRadiology website (rights confirmed by stakeholder).
- **Animation intensity**: moderate.
- **Aspect ratio**: 16:9.
- **Visual mode**: light clinical.
- **Typical deck size**: ~20 slides.
- **Must-have slide types**:
  - title,
  - agenda,
  - problem → solution,
  - flow.
- **Visual slots needed**: dedicated placeholders/regions for image and diagram embedding.
- **Persistent branding rule**: no always-on logo; include the **radial red rings** motif on all slides.
- **Content-over-background preference**: use visually raised text panels/cards over background graphics (high-contrast overlay surfaces with subtle shadow/elevation), similar to the provided Reveal.js example style.
- **Deliverables**: both reusable theme + starter project.

## Design direction (implementation-ready)

### Visual language
- Clinical, clean, white-first backgrounds.
- Strong hierarchy with generous spacing.
- Red accent strategy driven by easyRadiology radial ring motif.
- Subtle neutral tones for body content and supporting UI elements.
- Elevated content containers over visual backgrounds to preserve readability and create depth.

### Motion language (moderate)
- Use purposeful Reveal.js transitions and fragments:
  - fades for text blocks,
  - staggered item reveals,
  - controlled slide/zoom emphasis for section changes.
- Avoid heavy or distracting effects that compete with spoken delivery.

### Brand motif system
- Build reusable background utility classes so radial red rings appear consistently:
  - corner ring variant,
  - side ring variant,
  - low-opacity watermark variant.
- Keep motif subtle enough to preserve readability on dense content slides.

### Elevated text-over-graphics pattern
- Implement reusable “raised panel” classes for text over imagery/iframe/diagram backgrounds:
  - semi-opaque surface tokens (light and dark variants),
  - border radius and spacing tokens,
  - layered shadow presets for depth,
  - max-width rules and responsive placement utilities (left/right/center anchoring).
- Ensure WCAG-minded contrast and readability for projected conference environments.

## Slide system for a ~20-slide conference narrative

### Core required templates
1. Title / opening statement
2. Agenda
3. Problem statement
4. Solution framing
5. Flow/process (horizontal or vertical)

### Recommended supporting templates
6. Section divider
7. Key insight / quote
8. Metric highlight
9. Architecture/diagram slot
10. Image showcase slot
11. Summary
12. Final CTA / contact

## Build scope

### Deliverable A — Reusable theme package
- Custom CSS theme tokens (color, spacing, type scale).
- Utility classes for ring motif backgrounds and content containers.
- Animation utility classes for repeatable fragment behavior.
- Reusable elevated overlay/panel classes for text-over-graphics slides.

### Deliverable B — Starter deck
- 20-slide sample deck structure using the above templates.
- Placeholder copy in English.
- Placeholder blocks for image and diagram insertion.
- At least 2 example slides demonstrating raised text panels over background graphics.

## Asset usage plan
- Pull approved visual assets from easyRadiology site sources provided/confirmed by stakeholder.
- Normalize assets into project directories (e.g., `assets/images`, `assets/icons`, `assets/brand`).
- Preserve visual consistency (sizing, margins, contrast) across slide variants.

## Non-functional requirements
- Readability-first typographic scale suitable for conference projection.
- Motion should degrade gracefully if disabled.
- Maintain export compatibility for standard Reveal.js print/PDF workflows.
- Keep overlay effects performant and consistent across modern browsers.

## Open clarifications (to confirm before final polish)
1. Preferred font family if not inherited from sourced assets.
2. Whether to include slide numbers in footer when logo is omitted.
3. Whether flow slides should default to horizontal or vertical layout.

## Next step
Implement the Reveal.js theme and starter deck according to this locked specification, then review with stakeholder for visual fine-tuning.
