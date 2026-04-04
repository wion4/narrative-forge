---
name: story
description: Launch narrative design workflows — create stories, write dialogues, build worlds, design characters, or generate concept art
argument-hint: "[create|dialogue|world|character|concept|review]"
allowed-tools: ["Bash", "Read", "Write", "Edit", "AskUserQuestion", "Agent"]
---

Launch Narrative Forge workflows.

## Modes

- **No arguments / `create`**: Start a new story from scratch using story-architect agent
- **`dialogue`**: Write dialogue for a scene or character using dialogue-writer agent
- **`world`**: Build world lore, environmental storytelling, codex entries using world-narrator agent
- **`character`**: Design a character or ensemble using character-builder agent
- **`concept`**: Generate 2D concept art using concept-artist agent
- **`review`**: Review existing narrative content against the methodology

## Execution

1. Detect system language: `echo $LANG`
2. Load the narrative-forge skill for methodology context
3. Launch the appropriate agent based on the mode
4. All agents should work in the user's language

## Review Mode

When user runs `/narrative-forge:story review`:

1. Read the narrative content the user points to
2. Check against methodology from SKILL.md:
   - Is there a clear core question?
   - Do characters have want/need/flaw?
   - Are there dead choices?
   - Is exposition shown or told?
   - Does environment tell stories?
   - Is dialogue differentiated?
3. Provide specific, actionable feedback with references to techniques
