# Replicate Android Feature

[![skills.sh](https://skills.sh/b/addxing/replicate-android-feature)](https://skills.sh/addxing/replicate-android-feature)

An agent skill for reproducing an existing Android feature in another project or platform. It treats the Android implementation as the source of truth and preserves the complete feature path, behavior, UI, and reusable resources.

## Install

```bash
npx skills add addxing/replicate-android-feature
```

### DeepSeek Harness

This repo follows the DeepSeek Harness (DSH) Skill format. Clone it into a skills directory and it will be auto-discovered:

```bash
# User-level install (available in all projects)
git clone https://github.com/addxing/replicate-android-feature ~/.dsh/skills/replicate-android-feature

# Project-level install (current project only)
git clone https://github.com/addxing/replicate-android-feature .dsh/skills/replicate-android-feature
```

DSH hot-reloads the skills directory after cloning; the skill becomes available in new sessions.

## Usage

Ask your AI coding tool to apply the skill and identify the feature to reproduce:

```text
Use $replicate-android-feature to reproduce the favorites feature from the Android source project in the target project.
```

Provide the source and target project locations when they cannot be inferred from the workspace.

## What It Does

This skill guides an agent to:

- reproduce all Android functionality and business logic
- match all visual elements, including layout, colors, typography, and spacing
- trace and implement every feature entry and related page from the Android source code
- reuse Android resources, converting only formats unsupported by the target platform
- summarize implemented content, main changed files, validation, and remaining gaps or blockers

## Files

- `SKILL.md` - skill instructions
- `LICENSE.txt` - Apache 2.0 license
