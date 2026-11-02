# Jaba

Minimal React + TypeScript app with Vite, Tailwind CSS, and shadcn/ui (Base UI / Nova).

## Setup

Requires Bun and Node.js satisfying `^20.19.0 || >=22.12.0`.

```sh
bun install
bun run dev
```

## Commands

- `bun run dev` — start the development server.
- `bun run lint` — lint JavaScript, TypeScript, and React with Oxlint.
- `bun run build` — type-check and build for production in `dist/`.
- `bun run preview` — serve the production build locally.

## UI

Use Tailwind utilities for styling. Theme tokens live in `src/index.css`.
The shadcn Button lives in `src/components/ui/button.tsx`; `cn` is in `src/lib/utils.ts`.
Use `@/` to import from `src/`.

Add more shadcn components as needed:

```sh
bunx shadcn@latest add input
```

Oxlint replaces ESLint so the starter can use TypeScript 7 without the current
`typescript-eslint` peer dependency restriction.
