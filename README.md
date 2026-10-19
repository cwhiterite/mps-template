# mps-template

A GitHub template that bootstraps new projects with Matt Pocock's engineering skills installed and pre-configured — so every project you start inherits the workflow instead of rebuilding it.

## What you get

- **The skills** — 38 engineering & productivity skills (triage, to-tickets, to-spec, wayfinder, grilling, and more), pinned in `skills-lock.json`
- **Agent conventions** — `AGENTS.md` plus `docs/agents/` (issue tracker, triage labels, domain docs)
- **Room to grow** — custom workflow skills live in `.agents/skills/` and ship with every project created from this template

## Make it yours

1. **Use this template** — click **Use this template** on GitHub (or `gh repo create --template cwhiterite/mps-template`)
2. **Point the issue tracker at your repo** — in `docs/agents/issue-tracker.md`, replace the `<owner>/<repo>` placeholder with your new repo
3. **Start working** — ask `ask-matt` to route you to the right skill for whatever you're doing

To refresh the skills to the versions pinned in `skills-lock.json`, run `npx skills@latest install`.

## Adding a custom skill

Only add a custom skill when no existing skill already covers the task — check with `ask-matt` first. When you do, add it at `.agents/skills/<name>/SKILL.md`. Because `.agents/skills/` is tracked, your custom skill ships to every project created from this template.
