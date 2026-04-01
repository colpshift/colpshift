# Design Spec: GitHub Profile README

**Date:** 2026-03-31
**Owner:** Marcos Colpani (Colps)
**Repo:** colpshift/colpshift

---

## Goal

Replace the existing README.md with a production-ready GitHub profile page that establishes dual identity as Developer + AI Engineer, with a dark-theme aesthetic, minimal emoji use, and all text in American English.

## Layout (Option A — Two-column stats)

### 1. Header
- Typing SVG animation cycling 3 phrases (4s each, loop):
  1. `"Your most valuable skill isn't what you know. It's how quickly you learn what you don't."`
  2. `"Developer & AI Engineer"`
  3. `"Building intelligent integrations on ServiceNow + Angular"`
- Subtitle: `São Paulo, Brazil · AI-first workflow · Claude Sonnet 4.6`

### 2. About
- 4 sharp first-person lines covering: ServiceNow+Angular dev identity, AI Engineer angle (MCP/A2A/RAG in production), daily environment (CachyOS/Fish/Claude Code), and a closer tied to the quote theme.

### 3. Tech Stack
Flat-square Shields.io badges grouped:
- **Languages:** JavaScript, Python, Fish Script
- **Frameworks & Platforms:** Angular, ServiceNow, Node.js
- **AI & Tools:** Claude Code, MCP, RAG, Generative AI, VS Code
- **OS & Environment:** Linux (CachyOS), Fish Shell

### 4. AI Focus *(standout section)*
Framed prose section (not a badge dump). Lists: MCP, A2A, RAG, Deep Learning, Generative AI. One sentence on Claude Code daily workflow.

### 5. GitHub Stats (two-column)
- Left: `github-readme-stats` — dark theme
- Right: `streak-stats.demolab.com` — dark theme
- Below: `top-langs` compact card — dark theme

### 6. Current Focus
3-bullet list: ServiceNow Yokohama + Angular patterns, AI agent integration (MCP/A2A), English + AI continuous learning.

### 7. Connect
Three inline flat-square badges: LinkedIn · GitHub · X/Twitter

### 8. Footer
`capsule-render` wave banner with tagline: `"The model is the tool. The engineer is the edge."`

## Style Rules
- All shields: `style=flat-square`
- Stat cards: `theme=dark` or `theme=dracula`
- HTML centering via `<div align="center">` where needed
- Max 1 emoji per section header, used purposefully
- No filler phrases, no generic "passionate developer" copy
