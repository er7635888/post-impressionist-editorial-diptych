---
name: post-impressionist-editorial-diptych
description: Transform an uploaded photo into a vertical upper-lower editorial diptych with the original, unstyled photograph above, a sparse photo-derived abstract oil-painting memory panel below, and one poetic English title. Use when the user wants an original-photo-plus-abstraction composition, asks to keep the upper image unchanged, wants the lower abstract panel to feel like oil paint, or invokes this skill for the established upper-lower layout.
---

# Original Photo Editorial Diptych

Create one finished raster image from one uploaded photograph. Keep the source photograph visually unchanged in the upper section and pair it with a sparse abstract oil-painting memory panel below.

## Required Reference

Before generating, read [references/generation-spec.md](references/generation-spec.md). Use it as the prompt compiler and quality gate.

## Workflow

1. Inspect the uploaded photograph.
   - Identify 3-6 spatial facts: main subjects, scale, axes, foreground/background, repeated rhythms, color roles, and negative space.
   - Decide which facts should become abstract marks in the lower panel.

2. Build the upper scene.
   - Place the original uploaded photograph itself in the upper section.
   - Preserve its photographic appearance, composition, subjects, color, lighting, texture, and detail.
   - Do not redraw, repaint, stylize, abstract, filter, color-grade, retouch, extend, or add content to it.
   - Allow only proportional scaling and a minimal crop when needed to fit the upper section; never stretch or distort it.

3. Build the lower abstract panel.
   - Use a neutral ivory panel with generous whitespace.
   - Reconstruct only photo-derived relationships as sparse oil-painted marks, not a miniature illustration.
   - Give the marks visible oil-painting qualities: loaded brush edges, slight impasto thickness, broken color, and hand-painted pigment texture.
   - Use one primary mark family and at most two supporting mark families.

4. Add exactly one English title.
   - Place it only in the lower panel, usually lower-left or below the abstract motif.
   - Use a restrained editorial serif face in dark blue-gray, blue-green, charcoal, or another photo-derived dark color.

5. Generate the image with the built-in image generation tool.
   - Use the uploaded image as a reference image.
   - State explicitly that the upper section must reproduce the source photograph faithfully and must remain photographic.
   - Do not stop at a prompt-only answer unless the user explicitly asks for prompt-only.

6. Check the result.
   - Confirm the output is a vertical upper-lower diptych, not a single full-frame painting.
   - Confirm the upper section still looks like the original photograph, with no painterly or abstract treatment.
   - Confirm the lower panel is abstract, sparse, traceable to the photo, and visibly oil-painted.
   - Regenerate once with a stricter prompt if the output alters the upper photograph, loses the lower panel, or invents content.

## Output

Return the generated image. If useful, add one short note naming the title and the main relationships preserved.
