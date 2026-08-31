# maxwarnock.github.io

Portfolio site for Max Warnock — Earth data analytics, GIS, and remote sensing
projects. Built with [Jekyll](https://jekyllrb.com/) and served by GitHub Pages.

**Live:** https://maxwarnock.github.io

## Running locally

Requires Ruby and Bundler.

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000. The site rebuilds automatically as you edit.

## Layout

The site is a single page: `index.md` holds the bio and a list of project
cards, each linking to a project write-up in `projects/`.

| Path          | Contents                                                            |
| ------------- | ----------------------------------------------------------------- |
| `index.md`    | Home page — bio and the project card list                          |
| `projects/`   | Per-project write-ups (`.md`) and exported analysis notebooks (`.html`) |
| `_layouts/`   | `default.html` — the sidebar + ribbon page shell                   |
| `assets/css/` | `style.scss` — imports the `jekyll-theme-minimal` theme            |
| `img/`        | Photos, figures, card thumbnails (`*_cover.png`), and embeddable interactive plots |
| `maps/`       | Cartography and coursework map exports                             |
| `_config.yml` | Site title, theme, sidebar description                             |

## Adding a project

1. Add the write-up under `projects/` as `<slug>.md`.
2. Add a square cover image to `img/`, named `<slug>_cover.png`.
3. Add a card for it to the list in `index.md`.

## Deploying

Pushing to `main` triggers a GitHub Pages rebuild automatically; the live site
updates a minute or two later.

## Notes

- `projects/clustering-portfolio-post.html` is a large exported notebook and is
  intentionally left as-is.
