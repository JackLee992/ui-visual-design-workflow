# ui-visual-design-workflow

Standalone Codex skill repository for `ui-visual-design-workflow`.

## Contents

- `SKILL.md`: Main skill definition and workflow.
- `agents/openai.yaml`: Agent prompt wiring for this skill.
- `references/source-map.md`: Source map and reusable guidance.
- `references/visual-checklists.md`: Visual QA checklist.
- `references/game-image-generation-samples.md`: Game image generation sample prompts and QA notes.
- `assets/samples/`: Sample generated images used by the game image prompt examples.

## Usage

Copy this folder into your Codex skills directory, for example:

```bash
mkdir -p ~/.codex/skills/ui-visual-design-workflow
cp -R . ~/.codex/skills/ui-visual-design-workflow/
```

Then invoke the skill in a prompt:

```text
Use $ui-visual-design-workflow to review this app screen.
```
