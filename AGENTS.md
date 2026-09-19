# Agent rules — tech-demos monorepo

You are building inside a sticky demo monorepo. Follow these rules strictly.

## Scope

- Only add or update files under `apps/<kebab-slug>/` for the assigned demo.
- Do not create a new GitHub repository.
- Do not modify other apps, root tooling, or `tracking/` unless the task explicitly says so.
- Before coding, read `skills/project-planning/SKILL.md` and write/update `apps/<slug>/PLAN.md`.

## App requirements

- Self-contained: from `apps/<slug>/`, `bun install && bun run dev` must start the demo.
- Prefer Bun + TypeScript + Vite (or the stack named in PLAN.md).
- Keep the MVP small: one clear demo angle, not a product.

## Validation (required)

- Open one pull request.
- Attach **both** at least one screenshot AND at least one video of the running app in the PR (validation artifacts). Not optional.
- Describe how to run the app in the PR body.

## Model preference

Initial prototypes: Claude Fable 5 (`claude-fable-5`) unless the owner asks otherwise.
