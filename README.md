# research-writing-toolkit

A personal Claude Code plugin bundling nine skills for academic research writing.

## Skills

| Skill | Purpose |
|---|---|
| `literature-review` | Systematic literature reviews across academic databases |
| `scientific-writing` | IMRAD manuscript drafting in flowing prose |
| `section-writing-agent` | Per-section paper drafting (PaperOrchestra Step 4) |
| `citation-verification` | Verify references and prevent fake citations |
| `results-analysis` | Strict statistical analysis and result interpretation |
| `writing-anti-ai` | Remove AI writing patterns from prose |
| `peer-review` | Structured manuscript and grant review |
| `paper-self-review` | Pre-submission quality checks |
| `review-response` | Draft rebuttals and responses to reviewer comments |

## Install (Claude Code CLI)

```
/plugin marketplace add <git-url-or-local-path>
/plugin install research-writing-toolkit@research-writing-toolkit
```

Or copy/symlink the contents of `skills/` into `~/.claude/skills/`.

## Install (Cowork via MCPmarket)

Add this repository as a plugin marketplace in your MCPmarket workspace, then
run `/mcpmarket-my-toolkit:sync` in Claude Code.

## Attribution

These skills are bundled from upstream MIT-licensed sources:

- `literature-review`, `scientific-writing`, `peer-review` — from
  [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)
- `citation-verification`, `results-analysis`, `writing-anti-ai`,
  `paper-self-review`, `review-response` — from
  [Galaxy-Dawn/claude-scholar](https://github.com/Galaxy-Dawn/claude-scholar)
- `section-writing-agent` — from
  [Ar9av/PaperOrchestra](https://github.com/Ar9av/PaperOrchestra)

All original copyrights and licenses remain with their respective authors.
