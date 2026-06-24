---
name: rabrat-illustrations
description: Generate reusable RaBrat V1.2 fantasy raccoon article illustrations, 1:1 square Xiaohongshu cards, 16:9 body illustrations, shot lists, and image prompts for Chinese or English articles, methods, workflows, diagrams, SOPs, education explainers, and abstract concepts. Use when the user asks for raccoon article illustrations, RaBrat/Rabrat illustrations, 幻熊屁孩/RaBrat 浣熊, one-eyed glowing-mask raccoon visuals, body illustrations, square social cards, shot lists, prompt design, or public reusable cartoon knowledge-worker illustrations using the default ChatGPT image generation model without private APIs.
version: 1.2
---

# RaBrat Illustrations V1.2

## Core Positioning

Create reusable RaBrat-style article illustrations and social cards. The output should explain an article's key judgment, workflow, structure, state, scientific concept, or metaphor as a clean comic-style body illustration.

This public version must not depend on private APIs, proprietary local assets, or a custom trained model. Use the default image generation model available to Codex/ChatGPT. If a richer image-to-image tool is available, reference images may be used, but the skill must still work from text prompts alone.

## Default Character: RaBrat V1.2

Use the V1.2 fantasy RaBrat identity by default. This replaces the older generic raccoon wording.

RaBrat is a fantasy sticker-like raccoon brat:

- Chubby compact body, huge rounded head, small rounded body.
- Cream/tan fur with black ears, black paws, black feet, and a striped tail.
- A very wide, thick black bandit mask covers the entire eye area like one black visor.
- Exactly one visible eye: a glowing white-yellow crescent/slit eye on the viewer-right side.
- The viewer-left eye is completely hidden in the black mask. Never show a second eye.
- Small black oval nose.
- Sly jagged black grin with large triangular teeth.
- Short rounded arms near the chest or operating tools.
- Strong black silhouette, cute-but-dangerous fantasy toy feeling.
- Mischievous, clever, strategic, slightly villainous but funny.

Never use a normal realistic raccoon, a generic cute raccoon, round eyes, two eyes, fluffy wildlife, glossy 3D mascot, or children's cartoon style. The face identity is mandatory: huge black visor mask, one glowing crescent eye, triangular-tooth grin.

## Load References As Needed

- `references/style-dna.md`: V1.2 visual style, color, text, ratio, and negative prompts.
- `references/composition-patterns.md`: article-illustration structures and metaphor options.
- `references/prompt-template.md`: V1.2 generation prompt templates.
- `references/qa-checklist.md`: inspection and iteration rules.
- `assets/examples/`: accepted example outputs for visual calibration only. Do not copy their exact compositions unless useful for a similar article.

## Workflow

### 1. Digest the article or task

Extract the core argument, cognitive turning points, and visualizable concepts. Do not illustrate evenly. Prioritize cognitive anchors: conflict, before/after, input-output loop, filtering, compression, support mechanism, role tension, failure point, scientific mechanism, or state change.

### 2. Produce a shot list when asked

If the user asks for analysis or shot list, do not generate images. Output each shot with:

- Placement or card purpose.
- Theme.
- Core meaning.
- Structure type.
- What RaBrat does.
- Suggested objects.
- Short labels.
- Recommended ratio: `1:1` for Xiaohongshu/social cards, `16:9` for article body illustrations unless the user specifies otherwise.

### 3. Generate images when asked

If the user asks to generate or make images, generate one image per shot. Each image should:

- Use RaBrat V1.2 as the action subject.
- Explain one idea only.
- Use a physical comic metaphor rather than a formal chart.
- Use sparse labels.
- Keep large white space.
- Default to 1:1 square for Xiaohongshu cards or when the user says cards/social posts.
- Default to 16:9 horizontal for article body illustrations.

Use `references/prompt-template.md` to build prompts. Always include the V1.2 character block, especially the single glowing crescent eye and black visor mask constraints.

### 4. Check and iterate

Use `references/qa-checklist.md`. Regenerate if RaBrat shows two eyes, loses the thick black visor mask, loses the glowing crescent eye, loses triangular teeth, becomes a normal raccoon, becomes too cute, becomes realistic, turns into a PPT diagram, or uses too many labels.

### 5. Save delivery

Save accepted images in the user's project as:

```text
assets/<article-slug>-rabrat-illustrations/
01-topic-name.png
02-topic-name.png
```

For Xiaohongshu/social cards, use:

```text
assets/<article-slug>-rabrat-xhs-cards/
01-topic-name.png
02-topic-name.png
```

Keep original generated files unless the user asks to replace them.
