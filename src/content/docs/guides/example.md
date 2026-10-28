---
title: Run and edit the docs
description: Install this repository, start the local documentation site, and check a production build.
---

## Start the project

From a terminal with Node.js and npm available:

```sh
git clone https://github.com/TurboTwitch0/starlight.git
cd starlight
npm install
npm run dev
```

Open the local URL printed by Astro. The development server normally starts at
`http://localhost:4321`; use the printed address if that port is already occupied.

## Edit a page

Open `src/content/docs/guides/example.md`, change its text, and save. The running
development server updates the page. Every documentation page needs a `title` in
its frontmatter; add a `description` to explain what readers will find.

To add a page, create a Markdown file under `src/content/docs/`. For example,
`src/content/docs/guides/deployment.md` creates `/guides/deployment/`. Add its slug
to the Guides section of `astro.config.mjs`. Pages under `reference/` are added
to the Reference sidebar automatically.

## Check the production output

```sh
npm run build
npm run preview
```

The build writes the static site to `dist/`. Open the preview URL printed in the
terminal, then check the homepage, sidebar links, and the page you edited before
deploying `dist/` to a static host.

If the build fails, fix the first reported file or configuration error and run
the build again. `npm run preview` serves an existing build; rebuild after making
changes you want to check there.

See the [command and file reference](/reference/example/) for the project layout.
