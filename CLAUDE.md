# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About This Repository

This is Colps's GitHub profile repository (`colpshift/colpshift`). The only deliverable is `README.md`, which GitHub renders automatically on the public profile page at https://github.com/colpshift. Theme: cinematic dark, identity is a ServiceNow/Angular developer learning AI (not an "AI Engineer" — see commit `3855e2b`).

## Structure

- `README.md` — the entire profile page (~155 lines). Raw HTML mixed with Markdown for layout control. Sections: header/typing banner, badges, Ecosystem Map (mermaid), AI Learning Journey, Stats, footer.
- `docs/superpowers/specs/` — design spec for the README (`2026-03-31-github-profile-readme-design.md`). Check it before restructuring.
- `.claude/` — local Claude Code settings only; not part of the profile.

## External Services Used in README

- **GitHub Stats:** `gh-readme-profile.vercel.app` — profile stats card
- **GitHub Streak:** `streak-stats.demolab.com` — contribution streak widget
- **Trophies:** `github-profile-trophy-xi.vercel.app` — profile trophy display
- **Badges:** `shields.io` — technology/tool badges
- **Banner:** `capsule-render.vercel.app` — header/footer wave banners
- **Typing animation:** `readme-typing-svg.demolab.com` — rotating tagline in the header
- **Activity graph:** `github-readme-activity-graph.vercel.app`

## Editing Guidelines

- Changes to `README.md` take effect after pushing to `main` on GitHub — there is no local preview step.
- Badge URLs follow the pattern: `https://img.shields.io/badge/<LABEL>-<COLOR>?style=for-the-badge&logo=<LOGO>&logoColor=<COLOR>`
- Stats widgets are driven by the GitHub username `colpshift` embedded in their URLs.
- The layout uses `<p align="center">` and `<div align="center">` HTML tags for centering — keep this pattern consistent.

## Gotchas

- **Capsule-render text:** never put a raw `&` in the `desc`/`text` params — it breaks the SVG XML parse and the image disappears. Use `·` instead.
- **Mermaid:** use `graph TD`; `mindmap` renders with unreadable text on GitHub. Keep node labels plain (no `&`, use "and").
- **Typing SVG:** the `lines=` param is `;`-separated and URL-encoded (`%27` apostrophe, `%C2%B7` for `·`, `+` for spaces).
- Third-party widgets are hosted on free Vercel instances and can go down or rate-limit; a blank card is usually the service, not the README.
- Validate after pushing by viewing the live profile, since GitHub's renderer sanitizes some HTML.

## Workflow

- Commit directly to `main` with conventional prefixes (`feat:`, `fix:`, `docs:`), as in the existing history.
- No build, lint, or test commands exist.
