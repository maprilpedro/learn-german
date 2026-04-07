# Skills System Details

## Setup
- Repo: `~/GitHub/SkillsCentralizedforClaude/`
- Symlink pattern: `ln -s ../../GitHub/SkillsCentralizedforClaude/<skill-name> ~/.claude/skills/<skill-name>`
- **Critical**: Creating a SKILL.md is not enough — the symlink MUST exist or the skill won't appear

## adhd-planner Skill
- File: `~/GitHub/SkillsCentralizedforClaude/adhd-planner/SKILL.md`
- Symlink created: 2026-03-04
- **Upgraded** in previous session to integrate Todoist + Google Calendar MCP
- Modes: plan, reflect, migrate, log, done, dopamine, **review** (new), **sync** (new)
- Key design: Suggest-Then-Approve protocol — NEVER modify Todoist/Calendar without user approval
- ADHD Analysis Rules: overload detection (>5 tasks/day), overdue triage, priority-to-energy mapping (p1→HIGH, p4→LOW), 3x reality check
- Persistence: Todoist = tasks, Google Calendar = time, local files = journal only

## body-doubling Skill
- File: `~/GitHub/SkillsCentralizedforClaude/body-doubling/SKILL.md`
- Symlink created: 2026-03-04
- Referenced by adhd-planner for accountability support

## Common Issue
- If a skill doesn't show up after creation, check `~/.claude/skills/` for the symlink
- New skills require a Claude Code restart to appear in the available skills list
