# anna-schmid.github.io

My academic site, built on the academicpages template (a fork of the Minimal Mistakes Jekyll theme). Live at https://anna-schmid.github.io. Thanks for visiting!

## Pages

Three real pages.

- `_pages/about.md` — home page, permalink `/`
- `_pages/research.md` — "Research" nav link, permalink `/research/`. Hand-written project cards.
- `_pages/talks.md` — "Where to find me" nav link, permalink `/talks/`. Hand-written, year-by-year list.
- `_pages/404.md` — GitHub's error page. Not in the nav, but needed.
- `_pages/markdown.md` — leftover theme cheat-sheet, kept for reference. Not linked anywhere.

Nav links live in `_data/navigation.yml`. Add or remove links there.

## Layout & styling

All styling is in this file: `assets/css/main.scss`, below the `@import` lines. That's where:

- Brand colors are set (`$brand-color`, `$background-color`, etc.)
- The font is set (Inter)
- The footer background image lives (`.page__footer::before`, currently `land_AI_2.png`)
- The `.project-card` styling for the Research page lives
- The avatar circle border is removed

**To change the footer photo:** swap the file in `images/`, then update the filename in `.page__footer::before` in `main.scss`.

**To change the profile photo:** update `avatar` under `author:` in `_config.yml` (currently `2025_git.png`).

**To change the bio photo:** edit `_data/authors.yml`.

## Config

`_config.yml` holds the site title, description, author bio, social links, and Jekyll build settings. Trimmed to what's actually used, collections, or social fields. A pre-cleanup copy is saved at `_config.yml.backup` if you ever want to see what used to be there.

## Adding content

- **New page:** add a `.md` or `.html` file to `_pages/`, give it a `permalink`, then add it to `_data/navigation.yml` to put it in the nav.
- **New research project:** add a new `.project-card` block inside `_pages/research.md`.
- **New talk:** add a bullet under the right year in `_pages/talks.md`.