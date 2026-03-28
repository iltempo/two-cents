# claude-lenses

Response modifier skills ("lenses") for Claude Code. Each lens overlays every answer with an extra perspective.

## Available lenses

| Lens | What it does |
|------|-------------|
| Roast | Appends a sharp roast about your question |
| Psychoanalyze | Appends a psychological micro-analysis of what your question reveals |
| Devil's Advocate | Challenges your approach with what could go wrong |
| ELI5 | Re-explains the answer as if you're five years old |
| Haiku | Appends a haiku summarizing the answer |
| Paranoid | Appends security and risk concerns about what you're doing |
| Mentor | Adds a teaching moment about the underlying principle or pattern |
| Time Traveler | Adds how this would have been done 10 years ago vs. 10 years from now |
| Rubber Duck | Reflects the question back to reveal what you were really trying to figure out |

## Install

```
/plugin marketplace add alexandergreim/claude-lenses
/plugin install claude-lenses@claude-lenses
```

Or test locally:

```
claude --plugin-dir ./path/to/claude-lenses
```

## Usage

```
/lenses
```

You'll be asked which lens to activate. Once chosen, it stays active for the rest of the conversation.

## License

MIT
