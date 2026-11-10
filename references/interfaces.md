# Website, Windows application, Android/mobile, vehicle and embedded UI

## Detect
- Generic SaaS component kit with unrelated hero gradients, floating orbs, glow, emoji icons, and equally sized cards.
- Core product identity, feature illustrations, character/state imagery, or scene art represented only by emoji, off-the-shelf glyphs, trivial geometric shapes, or fake image placeholders.
- Decorative widgets with no task, unclear primary action, hidden status or weak hierarchy.
- Unjustified corner radius/shadow/animation everywhere and no density adjustment to the product.
- Fake buttons, dead links, placeholder content presented as real, bad states (loading/error/empty).
- Tiny touch targets, poor keyboard/focus behavior, low contrast, overflowing labels or unusable layouts.

## Revise
- Begin with a real user task and the three most important information elements/actions.
- Pick density by task: operating dashboard can be dense; onboarding can be spacious. Do not impose an arbitrary global minimalist theme.
- Define reusable design tokens (type scale, colors, spacing, radii, motion), then vary composition deliberately.
- Match interaction to platform: browser, Qt/PySide6, Android Compose, or approved vehicle UI framework. Port design intent, not CSS blindly.
- Ensure accessible labels, focus states, target sizes, error/loading/empty states and localization as applicable.
- If the user's product has a character, brand or theme, preserve it rather than replacing it with generic monochrome.
- For visual identity, feature storytelling, character states, maps/scenes, and other image-led UI, apply `asset-first.md`: design, create, and integrate original context-specific assets. Keep familiar system icons for standard actions (back, close, search, settings) when clearer.

## Anti-AI UI audit
- Do not default to pale mint, pastel green, or emerald as accent colors. Use the product design system and explicit user or brand color choices; retain these colors when they are intentional and appropriate.
- Do not automatically add subtitles or descriptive paragraphs beneath headings. Keep text that helps users understand or act.
- Remove repetitive marketing copy while preserving the intended message and supported claims.
- Avoid repeating a centered heading, subtitle, and card grid in every section. Choose a layout that fits each section and its purpose.
- Preserve essential instructions, warnings, accessibility information, and existing functionality.
- Before delivery, audit these patterns, correct substantiated issues within scope, and verify the resulting interface when tools allow.
## Vehicle UI extra gate
- Prioritize driving safety: brief glance readability, low interaction burden, appropriate contrast, status clarity, no distracting motion.
- Respect supported Android Auto templates, app categories and platform policies; do not promise unrestricted car-screen replacement.
- Assess animation and custom video by the running context; driving-mode limitations outrank aesthetics.

## Verify
Run or render representative screens when tools allow. Check at least one compact and one target-sized viewport; verify major interactions and navigation. If only source code is available, classify visual claims as unverified.
