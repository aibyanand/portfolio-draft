# CLAUDE.md

Standing context for working on this project. This file is auto-loaded every
session when working in this folder.

## What this project is

Personal portfolio website for **Anand Shridhar Sawant** (Director, Power,
Performance & On-device Machine Learning). Single-page static site, no build
step, no framework — plain HTML/CSS/JS.

## File structure

```
index.html   - all page content/sections
style.css    - all styling (CSS variables for light/dark theme)
script.js    - theme toggle + footer year, no dependencies
README.md    - short repo description
docs/
  spec.md    - content/requirements spec for the site (source of truth for copy)
  CLAUDE.md  - this file
```

## Deployment

- Repo: `aibyanand/portfolio-draft` on GitHub (public).
- Hosted via **GitHub Pages**, serving the `main` branch root (`/`) — classic
  "legacy" Pages build, not a GitHub Actions workflow. No build step needed;
  pushing to `main` is enough to trigger a redeploy.
- Live URL: https://aibyanand.github.io/portfolio-draft/
- This is a **trial/draft repo**. The intended final destination is the root
  site `aibyanand.github.io` — do not assume this repo name is permanent.
- `gh` CLI is installed at `~/.local/bin/gh` (not on PATH by default in every
  shell — add `export PATH="$HOME/.local/bin:$PATH"` or call it by full path).
  Already authenticated as GitHub user `aibyanand`.
- Git commits here use the GitHub no-reply email
  `185603190+aibyanand@users.noreply.github.com` (GitHub rejects pushes that
  leak a private primary email — use the no-reply address for commit author).

## Conventions / things to keep consistent

- No external CDNs/fonts — system font stack only, keep the site dependency-free
  and fast.
- Light/dark mode via `prefers-color-scheme` + a manual toggle button that sets
  `data-theme` on `<html>`, remembered in `localStorage`.
- Content (bio, skills, links) should match `docs/spec.md`. If the user gives
  updated content in chat, update both `index.html` and `docs/spec.md` so they
  stay in sync.
- Currently only a GitHub link is listed under contact — no email/LinkedIn/
  projects yet (intentionally omitted per the user, as of the last content
  update — check `docs/spec.md` for current status before assuming this is
  still true).

## Workflow notes

- After editing site files: commit and push to `main`; GitHub Pages rebuilds
  automatically (takes roughly 30–60s). Verify with `curl -s -o /dev/null -w
  "%{http_code}" https://aibyanand.github.io/portfolio-draft/` → expect `200`.
- Don't push broken HTML/CSS without a quick local sanity check of the file
  contents first — there's no CI/build step to catch errors.
