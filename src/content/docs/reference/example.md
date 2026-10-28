---
title: Commands and project files
description: Commands, source locations, routes, and build output for this repository.
---

Run commands from the repository root.

| Command | Purpose |
| --- | --- |
| `npm install` | Install the dependencies declared in `package.json`. |
| `npm run dev` | Start Astro's development server with live updates. |
| `npm run build` | Generate the production site in `dist/`. |
| `npm run preview` | Serve the most recent production build locally. |
| `npm run astro -- --help` | Show the available Astro CLI commands. |

| Path | Purpose |
| --- | --- |
| `astro.config.mjs` | Site title, GitHub link, and sidebar configuration. |
| `src/content.config.ts` | Documentation content collection and schema. |
| `src/content/docs/index.mdx` | Homepage content and links. |
| `src/content/docs/guides/` | Task-based guides; add their slugs to the sidebar. |
| `src/content/docs/reference/` | Reference pages discovered automatically by the sidebar. |
| `src/assets/` | Images imported by content pages. |
| `public/` | Files copied to the output without processing. |
| `dist/` | Generated deployment output; edit source files instead. |

Documentation file paths determine page routes. For example,
`src/content/docs/reference/example.md` becomes `/reference/example/`.

Start with [Run and edit the docs](/guides/example/) for the complete local workflow.
