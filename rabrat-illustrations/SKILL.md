---
name: rabrat-illustrations
description: Generate reusable RaBrat-style raccoon article illustrations, shot lists, and image prompts for Chinese or English articles, methods, workflows, diagrams, SOPs, and abstract concepts. Use when the user asks for raccoon article illustrations, RaBrat/Rabrat illustrations, one-eyed clever raccoon visuals, body illustrations, shot lists, prompt design, or public reusable cartoon knowledge-worker illustrations using the default ChatGPT image generation model without private APIs.
---

# RaBrat Illustrations

## Core Positioning

Create 16:9 horizontal article illustrations using a reusable one-eyed clever raccoon character. The output should explain an article's key judgment, workflow, structure, state, or metaphor as a clean comic-style body illustration.

This public version must not depend on private APIs, proprietary local assets, or a custom trained model. Use the default image generation model available to Codex/ChatGPT. If a richer image-to-image tool is available, reference images may be used, but the skill must still work from text prompts alone.

## Character

Use RaBrat as a generic reusable article-illustration character:

- Raccoon knowledge worker, not a realistic animal.
- Big rounded head and compact body.
- Beige-gray face/body, black paws, small rounded ears, striped tail.
- Bold black bandit mask.
- Exactly one visible eye, sharp and calculating; the other eye is fully hidden by the black mask or eyepatch.
- Sly sideways grin with jagged triangular teeth.
- Cunning, clever, strategic, mischievous, slightly villainous but funny.
- More smart trickster than cute mascot.

Never show two visible eyes. Avoid baby-cute, fluffy, realistic, glossy mascot, 3D, or wildlife-photo styles.

## Load References As Needed

- `references/style-dna.md`: visual style, color, text, and negative prompts.
- `references/composition-patterns.md`: article-illustration structures and metaphor options.
- `references/prompt-template.md`: generation prompt templates.
- `references/qa-checklist.md`: inspection and iteration rules.
- `assets/examples/`: accepted example outputs for visual calibration only. Do not copy their exact compositions unless useful for a similar article.

## Workflow

### 1. Digest the article

Extract the article's core argument, cognitive turning points, and visualizable concepts. Do not illustrate evenly. Prioritize 3-8 cognitive anchors: conflict, before/after, input-output loop, filtering, compression, support mechanism, role tension, failure point, or state change.

### 2. Produce a shot list when asked

If the user asks for analysis or shot list, do not generate images. Output each shot with:

- Placement.
- Theme.
- Core meaning.
- Structure type.
- What RaBrat does.
- Suggested objects.
- Short labels.

### 3. Generate images when asked

If the user asks to generate or make images, generate one image per shot. Each image should:

- Be 16:9 horizontal.
- Use the one-eyed raccoon character as the action subject.
- Explain one idea only.
- Use a physical comic metaphor rather than a formal chart.
- Use sparse labels.
- Keep large white space.

Use `references/prompt-template.md` to build prompts.

### 4. Check and iterate

Use `references/qa-checklist.md`. Regenerate if the raccoon shows two eyes, becomes too cute, loses the black mask, becomes realistic, turns into a PPT diagram, or uses too many labels.

### 5. Save delivery

Save accepted images in the user's project as:

```text
assets/<article-slug>-rabrat-illustrations/
01-topic-name.png
02-topic-name.png
```

Keep original generated files unless the user asks to replace them.
