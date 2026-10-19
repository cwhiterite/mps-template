## Agent skills

### Issue tracker

Issues and specs for this repo live as GitHub issues. See `docs/agents/issue-tracker.md`.

### Triage labels

Default vocabulary, one label per role: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `GLOSSARY.md` and `docs/adr/` at the repo root. See `docs/agents/domain.md`.

### Custom skills

Before creating a custom workflow skill, check whether an existing skill already covers the task — `ask-matt` routes to the right skill. Only add a custom skill when nothing existing fits. Custom skills live in `.agents/skills/` and ship with this template to every consumer project.
