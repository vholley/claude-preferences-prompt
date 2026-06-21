# claude-prompts-and-skills

Personal Claude configuration: the preference prompt I run in Claude, plus portable skills I've built. Public so the pieces are easy to reference and reuse.

## Contents

### `Claude.md`

My Claude preference prompt. This is the content that goes in Claude's user preferences, not a repo-level `CLAUDE.md` that instructs agents working in this repository. It defines a persona, a strict writing-style policy aimed at suppressing common AI-prose tells, and rules for reasoning, tool use, task handling, accuracy and provenance, and a pre-send self-check. It's tuned for a senior practitioner working across data, software, finance, and logistics.

### `deslop/`

A portable skill that edits prose to remove the markers that make text read as AI-generated, while preserving meaning, intent, and approximate length. It works structural and discourse-level tells first, then rhetorical and sentence-level, then lexical and surface, and explicitly avoids "fixing" patterns that only look like AI. The goal is authentic writing rather than detector evasion.

- `SKILL.md`: the skill definition and editing contract.
- `references/ai-writing-tells.md`: the catalog of tells, organized by tier.
- `README.md`: standalone overview of the skill.

Invoke it in a Claude session with `/deslop`, or by asking to make text sound less like AI.
