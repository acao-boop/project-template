# Project template

Starting point for Andrew Cao's static research sites. Each project is its own repository, published by GitHub Pages at `https://acao-boop.github.io/<repo>/` and listed on the portfolio, https://andrewcao.org/.

## Start a project
1. On GitHub: **Use this template → Create a new repository** (public, owner acao-boop). Clone it in VS Code into `~/Projects/<repo>`.
2. Replace `REPO-NAME` and `PROJECT TITLE` everywhere (`site/index.html`, `site/404.html`, `CLAUDE.md`, `tools/preview/make_preview.py`).
3. Settings → Pages → Source: **GitHub Actions**. Push `main`; the site goes live in about a minute.
4. Make a 1200×627 `site/social-preview.jpg` and check it in LinkedIn Post Inspector.
5. Add the project to the portfolio, https://andrewcao.org/ (ask the ★ Portfolio · LEAD chat; the code is in the portfolio repo), and set this repo's About website to the live URL.

## What's here
- `site/` is the whole website, published as-is. Plain HTML, CSS and JavaScript; no build step. Keep links relative, because the site lives under `/<repo>/`; only `404.html` uses full `/<repo>/` paths.
- `tools/preview/` previews unpublished edits over the live site in Claude's built-in browser.
- `CLAUDE.md` holds the standing instructions; `HANDOFF.md` records where each session left off.
