# Track `.agents/skills/` so custom workflow skills ship with the template

This repo is a GitHub template that bootstraps new projects with the engineering skills pre-installed. We commit `.agents/skills/` in full rather than gitignoring it and restoring from `skills-lock.json`, because custom workflow skills live in that folder and must reach every consumer project created from the template. Out-of-the-box completeness for consumers wins over the leaner lock-regenerable alternative.

## Considered Options

- **Track the whole `.agents/skills/` folder** (chosen): everything — pinned skills and custom skills — ships with every instantiation; no restore step needed.
- **Gitignore and restore from `skills-lock.json`** (rejected): keeps the repo lean but silently drops custom skills from consumer projects, since the ignored folder never propagates.
- **Publish custom skills to a source repo and install via the skills CLI** (rejected): clean lock integration but adds a publishing workflow the maintainer doesn't want.
