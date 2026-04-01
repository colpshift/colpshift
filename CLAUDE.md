# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About This Repository

This is Colps's GitHub profile repository (`colpshift/colpshift`). The only meaningful file is `README.md`, which GitHub renders automatically on the public profile page at https://github.com/colpshift.

## Structure

- `README.md` — the entire profile page. Uses raw HTML mixed with Markdown for layout control (centered headings, badge images, stats widgets).

## External Services Used in README

- **GitHub Stats:** `gh-readme-profile.vercel.app` — profile stats card
- **GitHub Streak:** `streak-stats.demolab.com` — contribution streak widget
- **Trophies:** `github-profile-trophy-xi.vercel.app` — profile trophy display
- **Badges:** `shields.io` — technology/tool badges
- **Banner:** `capsule-render.vercel.app` — footer wave banner

## Editing Guidelines

- Changes to `README.md` take effect after pushing to `main` on GitHub — there is no local preview step.
- Badge URLs follow the pattern: `https://img.shields.io/badge/<LABEL>-<COLOR>?style=for-the-badge&logo=<LOGO>&logoColor=<COLOR>`
- Stats widgets are driven by the GitHub username `colpshift` embedded in their URLs.
- The layout uses `<p align="center">` and `<div align="center">` HTML tags for centering — keep this pattern consistent.
