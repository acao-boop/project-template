# PROJECT TITLE

Public: https://acao-boop.github.io/REPO-NAME/ (repo acao-boop/REPO-NAME). Part of Andrew Cao's portfolio, https://acao-boop.github.io/. Andrew's role: WRITE IT HERE.

## Session routine
- Read HANDOFF.md first. Then read only the files the task needs.
- One bounded task per session. Before stopping, update HANDOFF.md (state, last change, checks, next step) and commit.

## Run and check
- No build step. When a feature changes, test it at desktop and phone widths, keyboard-only, with reduced motion and dark mode.
- Keep page links relative; the site lives under `/REPO-NAME/`. Only 404.html uses full paths.

## Review, then publish (every session)
- Nothing goes live mid-session. Edit `site/` and commit as work lands.
- Andrew reviews in Claude's built-in browser: run `python3 tools/preview/make_preview.py`, open the live site in the browser pane, and run `tools/preview/preview.js` there. New images appear only after publishing.
- When Andrew approves: commit and update HANDOFF.md; Andrew pushes `main` from VS Code (Source Control > Sync). When the Actions run finishes, confirm the live files match `site/` (SHA-256), then `git tag -f published`. If the social card changed, rerun LinkedIn Post Inspector.

## Portfolio
- Credit line: "Designed and built by Andrew Cao" (adjust to the real role), with Andrew's open A mark small beside it, linking to https://acao-boop.github.io/. Never larger, never as the project's logo.
- Give the project its own identity; don't reuse the hub's look.
- When the project is published or changes substantially, update its entry on https://acao-boop.github.io/.

## Constraints
- Plain static HTML/CSS/JS only: no framework, build step, backend, login, tracking or paid service without Andrew's decision.
- Preserve collaborators' prose, citations, sources and credits. A visual change does not authorize editorial changes.
- No redundant descriptions, duplicate navigation, all-caps labels, decorative numbering or purposeless symbols.

## Working with Andrew
- Be direct and specific. Lead with the result. Report only checks you actually ran.
