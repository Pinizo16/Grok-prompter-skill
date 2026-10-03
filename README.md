# Grok Prompter

A reusable skill/plugin for creating and modifying precise prompts for Grok.

## Core principle

**Define WHAT must be achieved, not HOW it must be implemented.**

Grok should retain decision authority over the technical, analytical, research, or creative solution unless the user explicitly requires a specific method, technology, tool, format, architecture, file, API, or other implementation detail.

## Modes

### Create from scratch
Build a new prompt from the user's current request and available context.

### Modify the previous prompt
Preserve all still-valid requirements from the previous prompt and integrate the requested changes without unnecessarily rewriting unrelated content.

## Defaults

- Prompts are generated in English.
- Generated prompts explicitly require Grok to respond to the end user in Spanish.
- Exact user-provided identifiers, paths, URLs, values, terminology, and other important details are preserved.
- Essential missing information triggers focused questions rather than invented assumptions.
- Prompt detail scales automatically with task complexity.
- Relevant requirements, edge cases, validation, and preservation constraints are included when applicable.
- The final prompt is ready to copy and paste.

## Software-project requirement

Whenever Grok modifies a software/project codebase, the project README must be created or updated so it remains a persistent, accurate map of:

- the project's objectives;
- major systems/components;
- which files/directories are responsible for which responsibilities;
- important dependencies and relationships;
- important conventions needed for future maintenance.

## Code-comment requirement

Whenever Grok creates, edits, debugs, refactors, audits, or otherwise modifies code, the prompt includes professional comment requirements.

Comments must be simple, one line, and used only to distinguish sections or indicate a necessary data/value in the code. They must not narrate obvious code or become decorative/explanatory blocks.

## Versioning

The plugin currently follows semantic-style versioning in its plugin manifest. Every substantive update should increment the plugin version and be reflected in this repository.

## Repository as source of truth

This repository is the canonical source for the Grok Prompter skill. Changes should be committed here before or together with plugin updates.

## Structure

```
.
├── plugin.json
├── .codex-plugin/
│   └── plugin.json
├── assets/
│   ├── icon.png
│   └── logo.png
└── skills/
    └── grok-prompter/
        ├── SKILL.md
        ├── assets/
        │   └── icon.png
        └── agents/
            └── openai.yaml
```

## Current plugin

- Name: Grok Prompter
- Current plugin version: 1.0.4
- GitHub repository: Pinizo16/Grok-prompter-skill
