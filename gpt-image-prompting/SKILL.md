---
name: gpt-image-prompting
description: Builds strong image-generation prompts from reusable GPT-Image-2 style patterns such as scene layout, camera realism, text rendering, comparisons, and annotated visuals. Use when creating or refining prompts for image generation, especially for clean tech, editorial comic, product, portrait, infographic, or social-media visuals.
---

# GPT Image Prompting

Use this skill when the user wants better image prompts, visual style adaptation, or reusable prompt templates.

## Quick workflow

1. Identify the output type:
   - infographic / chart
   - product or ad visual
   - realistic portrait / lifestyle
   - editorial illustration
   - comparison / split-panel
   - annotated image
2. Pick one base pattern from `references/patterns.md`.
3. Fill the template from `references/templates.md`.
4. Keep the prompt concrete: subject, composition, lighting, texture, text, aspect ratio, style.
5. If text must be readable, say that explicitly.

## Prompt formula

Use this order when writing prompts:

```text
[format/output]
[main subject]
[composition/camera/framing]
[lighting + mood]
[materials/textures/details]
[text that must appear, if any]
[style constraints]
[aspect ratio / size]
```

## Rules

- Prefer concrete nouns over abstract adjectives.
- Ask for legible on-image text only when it matters.
- For realistic images, specify lens, light, skin/material texture, and scene behavior.
- For editorial visuals, specify hierarchy: headline area, focal object, background restraint.
- For brand-safe results, describe the look instead of naming protected styles when unnecessary.
- Keep first draft short-to-medium; expand only when detail clearly helps.

## Clean tech default

When the user wants a visual for a product, post, or explainer and gives no style, default to:
- clean tech aesthetic
- minimal composition
- soft neutral background
- crisp edges
- modern UI/product feel
- restrained palette with one accent color

## Editorial comic default

For longer stories or explainers:
- editorial comic look
- clear focal subject
- magazine-like composition
- expressive but not chaotic
- limited palette
- readable negative space for text overlays

## Language choice

- For English prompts, use `references/patterns.md` and `references/templates.md`.
- For Russian-facing work or Russian drafts, use `references/patterns-ru.md` and `references/templates-ru.md`.
- Keep final generation prompts in English if the target image model follows English prompts better, but use Russian notes/templates for planning.

## References

- Pattern library: `references/patterns.md`
- Ready templates: `references/templates.md`
- Russian pattern library: `references/patterns-ru.md`
- Russian ready templates: `references/templates-ru.md`
- Source notes: `references/source-notes.md`
