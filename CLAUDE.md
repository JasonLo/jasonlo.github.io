# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal website for Jason Lo (jasonlo.dev), built with Astro. Deployed to GitHub Pages via GitHub Actions on push to `main`.

## Key Details

- **Environment**: Bun
- **Framework**: Astro
- **Styling**: TailwindCSS
- **Build output**: `dist/` (gitignored)
- **CI**: GitHub Actions in `.github/workflows/publish.yml`
- **No tests or linting** configured in this project

Default to using Bun instead of Node.js.

- Use `bun <file>` instead of `node <file>` or `ts-node <file>`
- Use `bun test` instead of `jest` or `vitest`
- Use `bun build <file.html|file.ts|file.css>` instead of `webpack` or `esbuild`
- Use `bun install` instead of `npm install` or `yarn install` or `pnpm install`
- Use `bun run <script>` instead of `npm run <script>` or `yarn run <script>` or `pnpm run <script>`
- Use `bunx <package> <command>` instead of `npx <package> <command>`
- Bun automatically loads .env, so don't use dotenv.
