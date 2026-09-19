# PLAN — openui-chat

## Goal

Tiny Bun + React chat playground that streams **OpenUI Lang** into live React components (card / form / table), demoing [OpenUI](https://github.com/thesysdev/openui) (`@openuidev/react-ui`, `@openuidev/react-lang`).

Source pick: https://x.com/DanKornas/status/2100211596886704477

## Non-goals

- Full agent platform / auth / multi-user
- Production LLM ops
- Editing other monorepo apps

## Stack

- Bun
- Vite + React + TypeScript
- `@openuidev/react-ui`, `@openuidev/react-lang` (and `@openuidev/react-headless` if required by the UI package)
- Mocked OpenUI Lang stream by default so `bun install && bun run dev` works offline
- Optional LLM key later (env), not required for the happy path

## MVP scope

1. Chat-style UI with a send box.
2. Default path: play a canned/mocked streaming OpenUI Lang response that renders at least a **card**, a **form**, and a **table** via OpenUI React components.
3. Import OpenUI styles (`@openuidev/react-ui/styles/index.css` or current docs equivalent).
4. README in this folder with run instructions.

## File layout (suggested)

```
apps/openui-chat/
  package.json
  bun.lock (or bun.lockb)
  vite.config.ts
  index.html
  src/main.tsx
  src/App.tsx
  src/mockStream.ts
  README.md
  PLAN.md
```

## Run

```bash
cd apps/openui-chat
bun install
bun run dev
```

## Validation (required)

- One PR that only touches `apps/openui-chat/`
- Attach **at least one screenshot AND at least one video** of the running app
- PR body explains how to run it
