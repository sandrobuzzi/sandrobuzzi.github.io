# AGENTS.md

## Project Scope

This repository contains the source for `sandrobuzzi.com`, a personal website.

Current stack:
- Plain HTML
- Plain CSS
- Optional small JavaScript enhancements
- Static hosting

## Working Goals

Priorities for changes in this repo:
- Keep the code modular and easy to extend.
- Preserve a high-quality visual identity rather than generic template styling.
- Keep public website content separate from private CV material.
- Favor accessibility, performance, and mobile-first layouts.

## Content Rules

Public website content belongs in `content/`.

Current workflow:
- private draft content lives in `private/content/`
- public-safe content can later be promoted into `content/` when ready

Current private draft files:
- `private/content/profile-draft.yml`
- `private/content/projects-draft.yml`
- `private/content/publications-draft.yml`

Do not place sensitive information in public content files. Exclude:
- personal phone numbers
- exact street or office addresses
- private email addresses if they should not be public
- unpublished work details
- anything not suitable for a public Git repository

Private material belongs in `private/`, which is gitignored.

## Structure Conventions

Preferred project structure:
- `index.html` for the main entry page
- `styles/` for modular CSS files
- `scripts/` for small progressive-enhancement JavaScript
- `content/` for public structured data
- `assets/` for images, icons, and downloadable public files
- `private/` for local-only material

CSS should be split by responsibility:
- `styles/tokens.css`
- `styles/base.css`
- `styles/layout.css`
- `styles/components.css`
- `styles/sections.css`

## Design Direction

The site should feel:
- editorial
- technically rigorous
- minimal but not bland
- distinct from generic portfolio templates

Avoid:
- default system-looking UI
- overly dense landing pages
- decorative elements without purpose
- heavy JavaScript frameworks unless there is a clear need

## Editing Guidelines

When editing this repo:
- Prefer semantic HTML.
- Keep classes reusable and descriptive.
- Use design tokens for colors, spacing, and type decisions.
- Keep interactions lightweight and optional.
- Do not expose private CV information on the website.
- If adding new sections, make them easy to reorder or remove.

## Content Workflow

Recommended update flow:
1. Update draft data in `private/content/`.
2. Build or revise website sections from that local-only data.
3. Keep private CV edits inside `private/cv/`.
4. When the content is ready for publication, copy only sanitized fields into `content/`.
5. If a public CV is needed, generate it from sanitized content rather than the private CV source.
