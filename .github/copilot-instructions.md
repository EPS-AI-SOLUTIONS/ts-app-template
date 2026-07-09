# Copilot instructions — ts-app-template

This is a **Bun**-based TypeScript single-page app: Vite + React 19.2 + Tailwind 4 + Biome + Vitest (TypeScript 6.0). Follow these conventions.

## Package manager — Bun only
- Use **Bun** exclusively. The lockfile is `bun.lock`.
- **Never** run npm, pnpm, or yarn, and **never** create `package-lock.json`, `pnpm-lock.yaml`, or `yarn.lock`. Adding an npm/pnpm/yarn lockfile to this repo is a defect.
- Install/update dependencies with `bun install` / `bun add`.

## Commands
- `bun install` — install dependencies
- `bun run dev` — start the Vite dev server
- `bun run build` — typecheck + production build (`tsc -b && vite build`)
- `bun run lint` — Biome check (this repo uses Biome, not ESLint/Prettier)
- `bun run test` — run Vitest once
- `bun run typecheck` — `tsc -b --noEmit`

## Scope discipline
- Change **only** what the issue explicitly asks for. Do not add unrelated files, dependencies, configuration, or refactors.
- Keep the diff minimal and focused on the requested change.

## Template placeholders
- `TEMPLATE_APP_NAME` and `TEMPLATE_DESCRIPTION` are intentional placeholders. Do **not** replace them unless the task explicitly asks you to rename the app.
- `@eps-ai-solutions/ui` is intentionally absent (not yet published) — do not add it.

## Stack notes
- State management: Zustand 5. Animations: `motion`. React 19.2, TypeScript 6.0.
