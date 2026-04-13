# Analytics Gym

A personal, open reference: mental models I find useful, and lessons from building and shipping.

Kept in the open so I can point others to it and so past-me keeps teaching present-me. Built with Quarto, deployed on GitHub Pages.

## Live Site

[analyticsgym.github.io](https://analyticsgym.github.io)

## Sections

- **Mental Models** — frameworks I reach for when thinking about growth, experimentation, and analytical problems
- **Ship Notes** — what I learned from things I actually built, tested, or shipped

## Adding a New Post

1. Copy a template from `_templates/` into `posts/`
2. Rename the file (kebab-case: `my-post-title.qmd`)
3. Set `draft: false` when ready to publish
4. Push to `main` — GitHub Actions builds and deploys automatically

## Design

Styling lives in `styles.css`. Run `quarto preview` to verify changes locally before pushing.
