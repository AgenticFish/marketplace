# AgenticFish marketplace

Claude Code plugin marketplace for the [AgenticFish](https://github.com/AgenticFish) org.

## What's here

Just `.claude-plugin/marketplace.json` — the catalog of plugins. Currently lists one:

- **composir** (→ https://github.com/AgenticFish/composir) — popular-science writing workflow plugin

## Conventions

- **Marketplace name**: `agenticfish` (what appears after `@` when users install: `/plugin install <plugin>@agenticfish`)
- **Plugin sources**: GitHub (`AgenticFish/<plugin-name>`). Each plugin lives in its own repo.
- **Adding a new plugin**: create its repo under AgenticFish org, then add an entry to `.claude-plugin/marketplace.json` with `source: { "source": "github", "repo": "AgenticFish/<name>" }`
- Non-plugin AgenticFish repos are invisible to Claude Code — only the repos listed in marketplace.json matter.

## Related

For the actual plugin development work, see `AgenticFish/composir`. Its `CLAUDE.md` has the full architecture, design decisions, and development conventions.
