# CLAUDE.md

## Site Purpose

A personal, open reference: mental models I find useful, and lessons from building and shipping. Kept public so I can point others to it and so past-me keeps teaching present-me. Written for myself first — if it's also useful to a teammate or a stranger, good.

## Content Sections

**Mental Models** — Frameworks I reach for when thinking about growth, experimentation, monetization, and analytical problems. A living reference I add to over time. The thing I'd send someone to explain why I'd approach a problem a certain way.

**Ship Notes** — What I learned from things I actually built, tested, or shipped. Anchored to a real problem and the lesson I took from it. AI and automation show up here naturally as the accelerant, not as a standalone topic.

## Content Rules

- Topics tie to growth, experimentation, monetization, or the analytical/engineering craft behind them
- AI building is woven through Ship Notes as the how, not a standalone category
- Every post passes this filter: comes from real experience, useful to future-me or someone I'd share it with, and requires my specific background to write credibly

## Guardrail

If a content request drifts from this — wrong topic, no real experience anchor, generic advice anyone could write, or treats AI as a standalone subject rather than an accelerant — reject it or redirect back to the site purpose.

## Tech Stack

- Quarto website project, output dir `docs/`, deployed to GitHub Pages via GitHub Actions
- Single `posts/` directory for all content
- Two categories only: Mental Model, Ship Note
- No timestamps on any content — sort alphabetically
- Status taxonomy: seed | developing | mature

## Layout & Styling

- All visual styling lives in `styles.css` — single source of truth
- Custom header (`_includes/header.html`) replaces Quarto's navbar: site title + two tabs (Mental Models, Ship Notes), wired via `include-before-body` in `_quarto.yml`
- Default Quarto navbar and TOC are hidden via CSS
- Responsive breakpoints at 768px and 420px — verify both desktop and mobile when making layout changes

## Adding Content

1. Copy a template from `_templates/` (writing.qmd or notebook.ipynb)
2. Place in `posts/`
3. Write
4. Push to main — GitHub Actions builds and deploys automatically

## Local Preview

After making changes (content, styling, or config), run `quarto preview` to verify locally before pushing. Do not rely on production to test changes.

## Verifying Prod After Deploy

GitHub Actions typically deploys in ~40s. After a styling change, browser cache can mask the new CSS — hard-refresh (Cmd+Shift+R) or use an incognito window before concluding something is broken. If the deployed HTML and `styles.css` on the server look correct but the page renders old styles, it's cache, not the build.
