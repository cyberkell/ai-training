# Project instructions

## Session name
Sessions in this folder are named **AI Training**. A `SessionStart` hook in `.claude/settings.json` sets the title automatically (only when the session has no title yet, so a manual rename is kept). Don't remove it. If a session still shows another name, rename it with:

```
/rename AI Training
```

## Session color
Sessions here have a yellow prompt bar. No hook can set color, so `.claude/settings.json` sets `"agent": "ai-training"`, which runs the main session as the agent in `.claude/agents/ai-training.md` (`color: yellow`). Keep that agent file's body **empty**: an agent with instructions replaces the normal Claude Code system prompt, while an empty one keeps it (tested 2026-11-23 on v2.1.331). `/color` in a session still overrides it.
