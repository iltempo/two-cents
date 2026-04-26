# Two Cents

Claude Code skill plugin that adds unsolicited opinions to every answer.

## Release checklist

When modifying `skills/two-cents/SKILL.md`:

1. Bump `version` in `.claude-plugin/plugin.json` (current: 1.8.0)
2. Commit both files together
3. Push to trigger marketplace update

The plugin cache at `~/.claude/plugins/cache/` serves the published version — local edits won't take effect until republished.

## Local development

To test changes before publishing, symlink your local skill into the plugin cache:

```bash
ln -sf $(pwd)/skills/two-cents ~/.claude/plugins/cache/iltempo-claude-plugins/two-cents/dev/skills/two-cents
```

Then `/reload-plugins` and invoke `/two-cents`.

## Adding a mode

- Add a row to the Modes table in `SKILL.md`
- Tone: sharp (default) or soft (eli5, mentor only)
- Keep voice description under 25 words
- No per-mode examples needed — shared examples section covers the format

## Token budget

The skill loads into context every turn. Target: under 500 words.
