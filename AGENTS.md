# Repository Guidelines

## Project Structure & Module Organization
- `src/pages/`: Route-based pages (`.astro`, `.md`, `.mdx`). File names map to routes.
- `src/components/`: Reusable UI components.
- `src/layouts/`: Page layouts used by content and routes.
- `src/content/` and `src/content.config.ts`: Content collections and schema.
- `src/assets/` and `public/`: Local assets; `public/` is served at the site root.
- Config: `astro.config.mjs`, `tsconfig.json`.

## Build, Test, and Development Commands
- `npm install`: Install dependencies.
- `npm run dev`: Start the local dev server (default `http://localhost:4321`).
- `npm run build`: Build the production site into `dist/`.
- `npm run preview`: Serve the built site locally for a final check.
- `npm run astro -- --help`: Astro CLI help and subcommands.

## Coding Style & Naming Conventions
- Match existing formatting in `src/` and keep changes consistent with adjacent files.
- Use clear, descriptive component and file names (e.g., `Hero.astro`, `PostCard.astro`).
- Keep content files in `src/content/` aligned with the configured collections.
- No dedicated formatter or linter is configured; avoid large reformat-only diffs.

## Testing Guidelines
- No automated test suite is currently configured.
- Minimum checks before opening a PR: `npm run build` and a manual smoke test via `npm run preview`.

## Commit & Pull Request Guidelines
- Existing history uses short, simple messages (e.g., “Update”). Prefer concise, imperative summaries.
- PRs should include: a brief summary, key changes, and screenshots for visible UI changes.
- Link related issues or context when available.

## Security & Configuration Tips
- Do not commit secrets or local config; keep credentials outside the repo.
- When adding integrations, document required environment variables and defaults.
