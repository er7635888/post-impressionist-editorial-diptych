# Generation Spec

Use this spec to compile the final image-generation prompt.

## Composition Contract

Create one complete vertical editorial diptych:

- Upper principal image area: 42%-52% of final height.
- Lower abstract memory panel: 48%-58% of final height.
- Join the two sections directly with a clean flat edge.
- Do not use frames, drop shadows, tape, collage edges, mockups, borders, labels, signatures, logos, or watermarks.
- Do not create a single full-frame scene. The lower panel must be visibly separate.

## Upper Scene

Use the uploaded photograph as the only content source.

Place the original uploaded photograph itself in the upper area. Preserve:

- the source photo's photographic appearance and main composition
- the positions and scale relationships of important subjects
- foreground/background hierarchy
- distinctive axes such as horizon lines, roads, poles, boats, buildings, mountains, or shorelines
- original color, lighting, texture, sharpness, grain, and detail

Do not redraw, repaint, stylize, abstract, filter, color-grade, retouch, beautify, extend, or reinterpret the upper photograph. Do not add or remove objects. Permit only proportional scaling and the smallest necessary crop; never stretch or distort the photo.

## Lower Abstract Oil-Painting Memory Panel

Use a uniform neutral ivory background, close to `#F3F0E8`. The panel may show a subtle material surface only if it remains calm and uniform; avoid noisy paper texture, stains, gradients, glow, vignettes, or collage effects.

Reconstruct the source photo's relationships as abstract oil-painted marks:

- Use one primary mark family: low bands, geometric blocks, organic masses, arcing strokes, tapered strokes, short bars, or simplified masses.
- Use at most two supporting families: fine structural lines, small dots/blocks, restrained figure marks, repeated rhythms, or tiny identity cues.
- Keep 60%-80% of the panel as clean negative space.
- Place the motif in the lower-middle, centered, or slightly off-center according to the source composition.
- Make every mark traceable to a fact in the photo.

Oil-painting feel:

- Give the lower-panel marks visible brushwork, slight impasto thickness, loaded edges, and broken color.
- Let pigment show small variations inside each mark, especially in photo-derived highlight colors, dark silhouettes, water/sky bands, or warm accents.
- Keep the ivory ground mostly calm and flat; oil texture should live mainly in the abstract marks, not across the whole panel.
- Avoid photorealistic rendering, airbrushed gradients, digital vector flatness, and over-detailed illustration.
- Do not let the oil-painting treatment spread into the upper photograph.

Subject reduction rules:

- Landscapes: compress water, shore, mountain, sky, cloud, and island relationships into low bands and organic masses.
- Boats or vehicles: keep 2-3 planar marks; avoid windows, mechanical detail, or realistic shading.
- People: use a single irregular vertical mark or tapered block; do not draw faces, limbs, clothing, or separate heads.
- Architecture or structures: retain only 1-3 identity cues, such as mass, axis, arch, tower, roofline, or silhouette.
- Trees and clouds: use clustered organic masses, not detailed leaves or cloud texture.

The lower panel should read first as sparse abstract oil painting and only second as a memory of the photo.

## Title

Create exactly one English title, 2-5 words, grounded in visible facts from the photo.

Good title directions:

- a relationship between two visible subjects
- light or weather entering a place
- a small subject below or beside a large subject
- a spatial or motion fact translated poetically
- a direct but elegant description

Avoid empty titles such as `Memory`, `Dream`, or `Moment`; avoid tourist-poster language and location labels.

Title placement:

- only inside the lower panel
- lower-left safe area or below the abstract motif
- restrained editorial serif typeface
- dark photo-derived color, not pure black
- no subtitle unless the user explicitly asks

## Prompt Shape

Use this structure for the final prompt:

```text
Create one complete vertical editorial diptych from the uploaded photo as the only content source.

Upper image area: [height share]. Place the original uploaded photograph itself here. Keep it photographic and visually unchanged. Preserve [specific subjects and positions]. Permit only proportional scaling and the smallest necessary crop.

Lower abstract memory panel: [height share]. Uniform ivory background. Reconstruct only [3-6 source relationships] as sparse abstract oil-painted marks with visible brushwork, slight impasto thickness, loaded edges, and broken color. Use [primary mark family] plus [supporting mark families]. Keep [negative space amount].

Title: exactly "[title]" in the lower panel only, [placement and typography].

Constraints: [do not redraw, repaint, stylize, abstract, filter, retouch, extend, or alter the upper photograph; no extra objects; no text except title; no watermark; no single full-frame scene; no miniature illustration in the lower panel; oil-painting texture only in the lower abstract panel].
```

## Quality Gate

Before finalizing, check:

- Is the image a vertical upper-lower diptych?
- Is the upper area clearly the original photograph rather than a generated painting or abstraction?
- Does the upper area preserve the source composition, color, lighting, texture, and detail?
- Is the lower area an ivory abstract oil-painting panel, not another full scene?
- Are lower-panel marks sparse and traceable to photo facts?
- Do lower-panel marks show visible brushwork, slight impasto, loaded pigment edges, and broken color?
- Is there exactly one English title in the lower panel?
- Are there no extra labels, signatures, logos, dates, numbers, or watermarks?
