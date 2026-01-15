# Repository Guidelines

## Project Structure & Module Organization
This is a static-site repository with all content at the repo root.
- HTML pages live in the root (e.g., `index.html`, `website1.html`, `letter1.html`).
- Assets are also in the root (e.g., `*.png`, `*.jpg`, `*.jpeg`, `*.mp4`).
- `CNAME` configures the custom domain for hosting.
- `node_modules/` is present for tooling only (no runtime build step).

When adding new pages, follow the existing pattern of root-level HTML files and reference assets with relative paths like `./image.png`.

## Build, Test, and Development Commands
There is no build or dev server configured. Formatting is handled via Prettier:
- `npm run format` — formats all files in the repo using Prettier.
- `npm run format:check` — checks formatting without writing changes.

## Coding Style & Naming Conventions
- Indentation: follow existing HTML formatting; use Prettier for consistency.
- HTML files use lowercase, descriptive names (e.g., `website7.html`).
- Asset names are short and consistent with page usage (e.g., `website7.jpg`).

If you add new assets, keep names lowercase and avoid spaces. Prefer `kebab-case` or the current numeric pattern, and update HTML references accordingly.

## Testing Guidelines
No test framework is configured. If you need validation, rely on manual checks:
- Open HTML files in a browser to verify layout and asset loading.
- Run `npm run format:check` before commits.

## Commit & Pull Request Guidelines
Git history shows short, simple subjects (e.g., numbers or page names) and no enforced convention. Keep commits concise and descriptive, for example:
- `add website10 landing page`
- `update letter1 imagery`

For pull requests, include:
- A brief summary of changes.
- Links to any relevant issues (if used).
- Screenshots or screen recordings for visual changes.
