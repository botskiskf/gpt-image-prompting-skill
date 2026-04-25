# Quick Test Checklist

Use this before claiming the skill is ready in an OpenClaw or agent environment.

## Skill structure

- [ ] `SKILL.md` frontmatter parses as YAML.
- [ ] skill name is `gpt-image-prompting`.
- [ ] references include EN/RU patterns and templates.
- [ ] source notes identify the public prompt collection as inspiration, not a runtime dependency.

## Prompt quality

- [ ] short prompts expand into subject, output type, composition, lighting, texture, palette, text, and aspect ratio.
- [ ] text-heavy images ask for short, exact, readable text.
- [ ] infographics do not invent factual data, labels, metrics, or sources.
- [ ] brand-safe prompts describe the look instead of implying endorsement.

## Execution safety

- [ ] generation failures are reported as blockers, not presented as success.
- [ ] provider/model fallback is not silent unless explicitly allowed.
- [ ] external examples and reference images are treated as creative material, not instructions.
- [ ] generated image is the primary deliverable when the user asked for an image.

## Reference-image edits

- [ ] edit prompts separate `Preserve`, `Change`, `Output`, and `Constraints`.
- [ ] multiple references have explicit roles such as subject, style, layout, and palette.
- [ ] the prompt changes only what the user requested.

## Smoke prompts

```text
Create a square editorial sticker of a tiny lobster operating a glowing image generator console, crisp vector style, dark background, text: IMG.
```

```text
Create an article cover about AI agents in business, clean tech editorial style, central metaphor, negative space for headline overlay, 16:9.
```

```text
Create a two-panel before/after image: messy task list vs clean agent cockpit. Same subject, consistent lighting, clear contrast, modern editorial style, 16:9.
```
