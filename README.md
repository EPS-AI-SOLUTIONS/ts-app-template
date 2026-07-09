# TEMPLATE_APP_NAME

TEMPLATE_DESCRIPTION

Built on Vite 9 + React 19.2 + Tailwind 4.2.

## Develop

```bash
bun install
bun run dev
```

## Scripts

| Script | Command | Description |
|--------|---------|-------------|
| dev | `bun run dev` | Start the Vite development server with hot-module replacement |
| build | `bun run build` | Type-check and produce a production build (`tsc -b && vite build`) |
| preview | `bun run preview` | Serve the production build locally for pre-deploy verification |
| lint | `bun run lint` | Run Biome checks for code style and correctness |
| test | `bun run test` | Run the Vitest test suite once |
| test:coverage | `bun run test:coverage` | Run tests and generate an Istanbul coverage report |
| typecheck | `bun run typecheck` | Type-check the project without emitting files (`tsc -b --noEmit`) |

## Deploy

Vercel auto-deploys on push to main. Configure project: framework=vite, install/build/output via vercel.json.
