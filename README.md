# Personal Website

Source for `sandrobuzzi.com`.

## Repository Layout

- `index.html`: current site entry point
- `styles.css`: current stylesheet
- `content/`: future public structured content, when ready
- `private/`: local-only material such as full CV source and exports
- `AGENTS.md`: project-specific working instructions

## Content Strategy

For now, use `private/content/` as the working source of truth while the site is being drafted.

Current private draft content files:
- `private/content/profile-draft.yml`
- `private/content/projects-draft.yml`
- `private/content/publications-draft.yml`

Do not commit private or sensitive material. Full CV source, compiled CV files, and draft structured content should stay under `private/`.

## Suggested Next Refactor

Move from the current single stylesheet to:
- `styles/tokens.css`
- `styles/base.css`
- `styles/layout.css`
- `styles/components.css`
- `styles/sections.css`

This keeps design tokens, layout logic, reusable components, and section-specific styling separate.

## Local Development

This project is currently a static site with no build step.

Open `index.html` directly in a browser or serve the directory locally with a simple static file server if needed.
