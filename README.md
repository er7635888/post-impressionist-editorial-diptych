# Post-Impressionist Editorial Diptych

[中文说明](README.zh-CN.md)

## Introduction

`post-impressionist-editorial-diptych` is a ChatGPT/Codex skill for turning an uploaded photograph into a clean vertical editorial diptych.

The upper section keeps the original photograph visually unchanged. The lower section translates the source image into a sparse, photo-derived abstract memory panel with an oil-painting feel: visible brushwork, slight impasto thickness, loaded pigment edges, and broken color. The final image includes exactly one poetic English title in the lower panel.

This skill is designed for quiet editorial image experiments, visual memory studies, photo-plus-abstraction layouts, and restrained poster-like compositions.

## What It Does

- Preserves the uploaded photo in the upper panel without repainting, filtering, retouching, or restyling it.
- Builds a lower abstract panel from visible facts in the photo, such as subjects, axes, horizons, structures, light, color roles, scale, and negative space.
- Gives the lower panel a sparse oil-painted look while keeping the ivory background calm and mostly open.
- Adds exactly one English title, grounded in visible details from the photo.
- Enforces an upper-lower diptych layout instead of a single full-frame painting.

## Output Style

The generated image should have:

- Upper image area: original uploaded photograph, still photographic and visually unchanged.
- Lower memory panel: neutral ivory ground, sparse abstract oil-painted marks, 60%-80% negative space.
- Title: one short poetic English title, placed only in the lower panel.
- No borders, logos, watermarks, signatures, dates, subtitles, or extra labels.

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── icon.svg
└── references/
    └── generation-spec.md
```

## Installation

### Option 1: Install From ChatGPT Skills UI

If your ChatGPT or Codex environment supports importing skills from a GitHub repository:

1. Open the Skills page.
2. Choose the option to add or import a skill.
3. Use this repository URL:

   ```text
   https://github.com/er7635888/post-impressionist-editorial-diptych
   ```

4. Confirm that `SKILL.md` is detected at the repository root.
5. Install or enable the skill.

### Option 2: Install From a Downloaded Folder

1. Download this repository as a ZIP, or clone it locally:

   ```bash
   git clone https://github.com/er7635888/post-impressionist-editorial-diptych.git
   ```

2. Keep the folder structure intact. `SKILL.md` must remain at the folder root.
3. Import or upload the folder through your skills manager.
4. Refresh the Skills page if the newly installed skill does not appear immediately.

### Option 3: Local Skill Directory

If your Codex-style environment loads skills from local folders, place this repository folder in your personal skills directory according to your environment's instructions, then restart or refresh skill discovery.

## How To Use

You can invoke the skill by name:

```text
Use post-impressionist-editorial-diptych on this photo.
```

You can also trigger it naturally without naming the skill:

```text
Create an upper-lower editorial diptych from this photo. Keep the top as the original photo, and make the bottom a sparse oil-painted abstract memory panel with one English title.
```

Shorter prompts also work when the intent is clear:

```text
Use the original photo above and an oil-painted abstract panel below.
```

## Example Prompt

```text
Turn this uploaded image into a vertical editorial diptych. Preserve the original photograph in the top half. In the bottom half, create a restrained oil-painted abstract memory panel based on the photo's main shapes, colors, axes, and light. Add one poetic English title.
```

## Usage Notes

- The upper photo should remain photographic and visually unchanged.
- The lower panel should be abstract, sparse, and traceable to the source photo.
- Oil-painting texture should appear mainly in the lower abstract marks, not in the upper photograph.
- If the upper photo becomes painterly or the lower panel becomes a literal miniature scene, regenerate with stricter constraints.

## Main Skill Files

- [`SKILL.md`](SKILL.md): Core trigger description and workflow.
- [`references/generation-spec.md`](references/generation-spec.md): Detailed prompt compiler and quality gate.
- [`agents/openai.yaml`](agents/openai.yaml): UI metadata for supported skill environments.
- [`assets/icon.svg`](assets/icon.svg): Skill icon asset.

## License

This project is licensed under the [MIT License](LICENSE).
