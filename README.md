# RaBrat Illustrations

A public Codex skill for generating reusable one-eyed raccoon article illustrations from articles, workflows, methods, and abstract concepts.

RaBrat is a clever, sly, one-eyed raccoon knowledge worker. It turns ideas into simple comic metaphors: sorting machines, rope conflicts, presses, wobbly supports, and other low-tech visual explanations.

![RaBrat sorting machine](examples/01-grounded-sorting.png)

## What This Is

This repository contains a portable Codex skill:

```text
rabrat-illustrations/
  SKILL.md
  agents/openai.yaml
  references/
  assets/examples/
```

The public version uses the default ChatGPT/Codex image generation path. It does not require a private API, Dreamina account, custom model, or proprietary reference-image service.

## Install

Copy the `rabrat-illustrations` folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R rabrat-illustrations ~/.codex/skills/rabrat-illustrations
```

Then start a new Codex session and invoke:

```text
Use $rabrat-illustrations to make 4 article illustrations for this essay.
```

## Character Rule

The most important visual rule:

> RaBrat shows exactly one visible eye. The other eye is completely covered by a black mask or eyepatch.

Other stable traits:

- black bandit mask
- jagged triangular teeth
- sly sideways grin
- striped tail
- clever, strategic, slightly villainous but funny

## Example Outputs

### 1. Sorting research material

![Sorting research material](examples/01-grounded-sorting.png)

### 2. Definition conflict

![Definition conflict](examples/02-definition-conflict.png)

### 3. Core value press

![Core value press](examples/03-core-value-press.png)

### 4. Brand-management support

![Brand management support](examples/04-brand-management-triangle.png)

## Usage Pattern

Ask for a shot list first when the article is long:

```text
Use $rabrat-illustrations. Analyze this article and give me a 5-image shot list. Do not generate yet.
```

Generate when ready:

```text
Use $rabrat-illustrations. Generate the 4 strongest body illustrations from this article.
```

## Notes

- Keep labels short.
- Generate one image per idea.
- Avoid formal diagrams and PPT charts.
- Regenerate when the raccoon has two visible eyes.
