# PROJECT TITLE

Public: https://acao-boop.github.io/REPO-NAME/ (repo acao-boop/REPO-NAME). Part of Andrew Cao's portfolio, https://andrewcao.org/. Andrew's role: WRITE IT HERE.

## Session routine
- Read HANDOFF.md first. Then read only the files the task needs.
- One bounded task per session. Before stopping, update HANDOFF.md (state, last change, checks, next step) and commit.

## Run and check
- No build step. When a feature changes, test it at desktop and phone widths, keyboard-only, with reduced motion and dark mode.
- Keep page links relative; the site lives under `/REPO-NAME/`. Only 404.html uses full paths.

## Review, then publish (every session)
- Nothing goes live mid-session. Edit `site/`.
- Review locally: from `site/`, run `python3 -m http.server 8000` and open http://localhost:8000/. Check desktop and phone widths, keyboard-only, reduced motion and dark mode.
- As a fallback only, run `python3 tools/preview/make_preview.py`, open the live site in the browser pane, and run `tools/preview/preview.js` there. New images appear only after publishing.
- When Andrew approves, Claude commits, updates HANDOFF.md, and pushes `main`. When the Actions run finishes, confirm the live files match `site/` (SHA-256), then tag the deployed commit as `published` and push the tag. If the social card changed, rerun LinkedIn Post Inspector.

## Portfolio
- Credit line: "Designed and built by Andrew Cao" (adjust to the real role), with Andrew's open A mark small beside it, linking to https://andrewcao.org/. Never larger, never as the project's logo.
- Give the project its own identity; don't reuse the hub's look.
- When the project is published or changes substantially, update its entry on the hub, https://andrewcao.org/ (code in the enoch repo, `portfolio/`).

## Launch checklist (before the first publish)
- **Share card:** a 1200×627 `social-preview.jpg` that fits the project's own look, with full og: and twitter: tags on every page (each page's own title, description and URL; one shared image with a `?v=` date). The page `<title>`, og:title and twitter:title say the same thing. After publishing, check the image URL returns 200 and image/jpeg, then run LinkedIn Post Inspector.
- **Icons:** an SVG favicon and a 180 px `apple-touch-icon.png`, linked from every page.
- **404:** `404.html` in the site's style, with one `<h1>`. It returns status 404 and carries `noindex`.
- **Headings:** exactly one `<h1>` per page, and the visible title must read correctly to a screen reader (no drop-cap letter split off outside the `<h1>`).
- **Links:** run a link check over every page, including external sources. Bot-blocked sites (403/429/999) need a manual look, not a fix.
- **Credit and hub:** the credit mark links to https://andrewcao.org/, and the project has an entry on the hub.
- **No working files in `site/`:** everything in `site/` is public. Notes, scripts and drafts live in `docs/`.

## Constraints
- Plain static HTML/CSS/JS only: no framework, build step, backend, login, tracking or paid service without Andrew's decision.
- Preserve collaborators' prose, citations, sources and credits. A visual change does not authorize editorial changes.
- No redundant descriptions, duplicate navigation, all-caps labels, decorative numbering or purposeless symbols.

## Working with Andrew
- Be direct and specific. Lead with the result. Report only checks you actually ran.
