# Claude Skills

Custom skills for [Claude Code](https://claude.ai/code) — reusable instructions that extend Claude's behavior for specific tasks.

## What are skills?

Skills are markdown files stored in `.claude/skills/`. Claude Code loads them automatically and uses them when the task matches the skill's purpose.

## Skills in this repo

### `file-naming` — Final Deliverable Naming Convention

Enforces a consistent naming format for all final deliverable files:

```
DEPARTMENT OR COMPANY - SHORT NAME OF FILE - YYYYMMDD
```

**Examples:**
- `Marketing - Q2 Campaign Brief - 20260628.pdf`
- `Acme Corp - Executive Summary - 20260628.docx`
- `Finance - Budget Forecast FY27 - 20260628.xlsx`

**Trigger:** Ask Claude to name, save, rename, or finalize a file and it will apply this convention automatically — prompting you for any missing details before confirming the new name.

## Usage

Copy the `.claude/skills/` folder into your project root, or into `~/.claude/skills/` to make the skills available globally across all projects.
