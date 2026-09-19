---
name: project-planning
description: >-
  Use this before implementing a new apps/<slug>/ demo in the sticky tech-demos
  monorepo. Write PLAN.md, then implement only that scoped MVP.
---

# Project planning (tech demos)

## Goal

Turn one approved technology pick into a tiny, runnable MVP under `apps/<kebab-slug>/`.

## Steps

1. Confirm slug, demo angle, and success criteria from the approval chat / task prompt.
2. Skim the upstream library docs just enough to pick the smallest integration path.
3. Write `apps/<slug>/PLAN.md` with:
   - Goal (one paragraph)
   - Non-goals
   - Stack (Bun + …)
   - File layout
   - Run commands (`bun install`, `bun run dev`)
   - Validation: screenshot + video of the running app in the PR
4. Implement only what PLAN.md lists.
5. Open one PR; attach screenshot(s) and video(s); do not touch other apps.

## Constraints

- Self-contained app directory
- Mocked / offline-friendly path when an API key would otherwise block `bun run dev`
- No new GitHub repository
