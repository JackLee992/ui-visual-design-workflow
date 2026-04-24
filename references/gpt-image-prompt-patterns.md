# GPT Image Prompt Patterns

Use this reference when a user wants stronger image generation prompts, prompt variants, reproducible samples, UI mockups, posters, character sheets, or photorealistic image direction.

These patterns are distilled from current GPT-Image-2 community case collections such as `EvoLinkAI/awesome-gpt-image-2-prompts`; do not copy a specific prompt, artist, character, celebrity likeness, franchise identity, or output image. Extract the reusable structure.

## Core Prompt Stack

For final image generation, write prompts in this order:

1. **Task and medium**: say exactly what the output is, such as live-action film still, product photo, vertical poster, UI mockup, character sheet, infographic, social screenshot, or game key art.
2. **Canvas and crop**: set aspect ratio, orientation, platform crop, safe area, and thumbnail readability.
3. **Subject lock**: define who/what is primary, identity consistency, age/adultness when relevant, body/proportions, pose, expression, outfit, props, and invariants that must persist across frames.
4. **Composition**: describe focal path, foreground/midground/background, negative space, grid/module logic, perspective, and whether the image is single-frame, collage, card grid, or information layout.
5. **Camera and rendering**: use medium-specific language, such as 35mm film, CCD flash, DSLR macro, practical TV-drama set, vector poster, hand-drawn ink, product catalog, dashboard screenshot, or 3D mockup.
6. **Lighting and color**: specify key/fill/rim light, practical light sources, contrast, haze, color grade, palette roles, and value separation.
7. **Material and detail**: name textures, typography behavior, UI component density, fabric, paper, glass, metal, skin texture, grain, shadows, and imperfections.
8. **Text policy**: state exact in-image text and language if required; otherwise say no readable text, no watermark, no logo. For text-heavy images, define hierarchy and keep copy short.
9. **Negative constraints**: exclude wrong medium, copied IP, unwanted UI/text, explicit content, distorted anatomy, over-polished skin, clutter, unreadable text, and anything that breaks platform rules.
10. **Reproducibility**: save the final prompt as a `.prompt.txt` sidecar next to any accepted sample image.

## Mode Recipes

### Photorealistic Portrait Or Film Still

Prioritize camera realism over style labels:

- Camera: focal length, lens behavior, handheld/studio feel, grain, motion blur, bokeh, exposure.
- Scene: practical set or real location, background distance, visible light source, natural imperfections.
- Subject: pose, expression, wardrobe, makeup, skin texture, hair behavior, age/adultness when needed.
- Guardrail: explicitly exclude game CG, anime, 3D render, over-smoothed skin, copied actor likeness, or explicit nudity when the request is sensual.

### Poster, Key Visual, Or Social Cover

Start with the marketing job:

- Define the promise in one sentence: product, event, fantasy, conflict, benefit, or emotion.
- Keep one dominant visual hook, then supporting symbols/details.
- Reserve title-safe or logo-safe negative space when typography will be added later.
- State whether text is generated inside the image or added later in a design tool.

### UI Mockup Or Social Screenshot

Treat it like product design, not decoration:

- Name device/platform, viewport, UI density, navigation, cards, buttons, feed rows, overlays, and component states.
- Specify real screenshot constraints: pixel-aligned layout, readable labels, realistic status bars, consistent spacing, no lorem ipsum unless requested.
- For fake social/app screens, avoid real private data, deceptive claims, and exact brand impersonation unless the user has authorization.

### Infographic Or Dense Information Design

Use modular structure:

- Define title, hero visual, 4-8 content modules, labels, callouts, comparison blocks, scoring, timeline, or process steps.
- Ask for high information density without crowding: clear hierarchy, icons, thin dividers, consistent rounded modules, and enough margins.
- For educational material, keep factual claims conservative unless source data is supplied or verified.

### Character Sheet, Grid, Or Multi-Frame Output

Lock consistency:

- State same identity, same face, same proportions, same outfit, same palette across frames.
- Define each frame or panel role separately.
- Request clean separation between panels and avoid mixing body parts across panels.

### Product Or Object Photography

Make the product inspectable:

- Specify object, material, scale, label behavior, angle, lens, surface, reflection, shadow, and background.
- Keep branding generic unless the user owns or provides the brand.
- Exclude warped labels, unreadable tiny text, impossible reflections, and extra duplicate objects.

## Variant Strategy

When exploring, produce three prompt directions:

- **Stable**: safest production interpretation with clear medium and constraints.
- **High-impact**: stronger composition, lighting, contrast, or editorial energy.
- **Experimental**: unusual layout, collage, material treatment, or worldbuilding, while preserving the core brief.

Score each candidate 0-2 on: subject fidelity, medium fidelity, composition clarity, text/layout control, platform crop, originality, and safety.

## Common Failure Fixes

- Too generic: add concrete medium, camera, setting, action, material, and platform crop.
- Too game-like: remove glow/VFX/render terms; add practical set, natural shadows, lens, grain, fabric wrinkles, real skin texture.
- Too cluttered: reduce subject count, reserve negative space, lower background detail, and name one focal point.
- Bad text: shorten copy, specify exact language and hierarchy, or generate without text and add typography later.
- Identity drift across grids: repeat same identity/outfit/face/proportions and define every panel.
- Bad hands/anatomy: simplify pose, avoid extreme perspective, add hands visible and anatomically natural only if necessary.
- Style copying risk: use broad genre and medium descriptors; avoid living artists, exact franchise costumes, logos, or named characters.
