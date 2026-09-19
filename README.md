# tech-demos

Sticky monorepo for weekday X-bookmark tech demos.

## Layout

- `AGENTS.md` — rules for Cursor cloud agents
- `skills/project-planning/` — plan before build
- `apps/<slug>/` — one self-contained demo app per pick (`bun install && bun run dev`)
- `tracking/seen-bookmarks.json` — scout proposals / skips / builds

## Conventions

- Bun only
- Never create a new GitHub repo per demo
- Cloud agents only add/update `apps/<slug>/`
- Every PR must include at least one screenshot AND one video of the running app
