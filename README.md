# mbriggs-skills

A collection of Claude Code skills by Marshall Briggs.

## Installation

```
/plugin install github.com/MarshallBriggs/mbriggs-skills
```

## Skills

### playtest

Autonomous UX playtesting using Playwright MCP. Simulates user personas navigating your app in a real browser, captures screenshots, and produces structured feedback reports with bug documentation, UX evaluation, and competitive analysis.

**Requires:** [Playwright MCP server](https://github.com/anthropics/playwright-mcp) configured in your project.

**Quick start:**
```
/mbriggs-skills:playtest
```

**Features:**
- 4 built-in generic personas (new user, power user, impatient expert, complete beginner)
- Two test modes: scripted (fixed task list) or reactive (persona discovers tasks naturally)
- Project-local overrides for custom personas, evaluation criteria, and competitive analysis
- Structured output: per-task reports, UX debrief, bug rollup, SWOP analysis, priority action list
- Token-efficient: uses accessibility snapshots for navigation, screenshots only for reports

**Customization:** Create `.claude/playtest/config.md` in your project with your app's URLs, then optionally add custom personas and competitive landscape. See [templates/playtest/project_setup_guide.md](templates/playtest/project_setup_guide.md) for details.

## Adding Skills

Future skills will be added as new directories under `skills/`. Install the plugin once and new skills become available on update.

## License

MIT
