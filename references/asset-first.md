# Asset-first gate — purposeful original visuals, not emoji/icon shortcuts

## When to activate
Apply when a web/app/desktop/vehicle UI, slide, report, game, document or graphic needs visual **identity**, **explanation**, **mood**, **character**, **object/scene**, **state feedback**, or **brand storytelling**. The requirement is about visual purpose, not forcing an image into every screen.

## Detect unacceptable shortcuts
- Replacing a requested drawing, character, custom illustration, cover visual, state animation, themed button graphic, or explanatory scene with an emoji or a stock outline icon.
- Filling every feature card with the first available Lucide/Material icon, irrespective of the feature's real meaning or product style.
- Using generic clip art, repeated gradients, a flat circle with letters, or arbitrarily simple geometry as a substitute for an image the user clearly needs.
- Writing prompts, naming files or leaving placeholder blocks while claiming that visual assets have been created and integrated.
- Mixing unrelated art styles or ignoring existing brand/character references, licenses and provided assets.

## Decision rule: use the right type of visual
1. **Standard interaction control** (back, close, search, settings, play/pause, warning): prefer a recognizable platform-consistent system icon if it best supports use and accessibility. An emoji is normally not a suitable UI control.
2. **Product-specific identity, story, role, mood or character**: plan and create a custom asset or matching asset family. Do not fall back to a generic icon merely because it is quicker.
3. **Information or evidence**: use a real screenshot, verified photograph, data chart or precise diagram as appropriate. Never present generated imagery as real evidence.
4. **No information or visual value**: omit the decoration. Do not force a custom illustration just to make an area look fuller.

## Required creation workflow
1. **Visual inventory:** identify each place that needs an asset and why. Separate essential assets from optional decoration. Reuse existing, correct assets before making duplicates.
2. **Asset brief:** specify intended meaning, subject, original visual direction, intended placement, aspect ratio, target size/resolution, transparency, contrast/background, and required states/variants. Refer to supplied brand references, character sheets, and design constraints.
3. **Make the asset:** use an available image-generation/editing tool for illustration/raster, or author actual vector/SVG, drawing, chart or diagram files when appropriate. Favor coherent asset families over unrelated one-off images. For character animation, keep proportions, anchor points and identities consistent across frames. If no creation tool can make the required asset, flag it as missing; do not disguise the gap with emoji or a trivial placeholder.
4. **Integrate:** place the real asset file into the screen, slide, or component. Add appropriate alt text/semantics, layout constraints and source/license notes if relevant.
5. **Inspect:** verify file existence, dimensions, alpha/transparent edges, composition, legibility at actual display size, cropping, theme/background, consistent style, and app/slide rendering. For animations, verify frame order, transitions and continuity.
6. **Fix concrete problems** and recheck. Do not replace working user-supplied graphics simply to make the result more fashionable.

## Platform and safety constraints
- Vehicle/driving UI: visual differentiation never overrides low-distraction design, glance readability, supported UI templates or manufacturer/platform restrictions. Avoid animated decoration while driving.
- Accessibility: familiar actions must remain easy to recognize; do not sacrifice touch targets, contrast, labels or focus states for custom visuals.
- Copyright and branding: respect user-provided references and permissions; do not claim generated assets are licensed originals without checking.

## Completion test
An asset-first job is **not complete** merely because a prompt or list of assets exists. The needed asset files must be created, included in the deliverable, and checked as far as tools allow. If this is impossible, state exactly what is missing and which validation was not performed.
