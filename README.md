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

| Path              | Contents                                                          |
| ----------------- | ---------------------------------------------------------------- |
| `index.md`        | Home page and the project card list                              |
| `pages/`          | Section pages (`EDS-portfolio.md`, `GIS-portfolio.md`)           |
| `projects/`       | Per-project write-ups and exported analysis notebooks (`.html`) |
| `_layouts/`       | Page templates (`default.html`, `project.html`)                  |
| `assets/css/`     | `style.scss` — imports the `jekyll-theme-minimal` theme          |
| `img/`            | Photos, figures, card thumbnails (`*_cover.png`), and embeddable interactive plots |
| `maps/`           | Cartography and coursework map exports                           |
| `_config.yml`     | Site title, theme, sidebar description                           |

## Adding a project

1. Add the write-up under `projects/`.
2. Add a cover image to `img/` (square, named `<slug>_cover.png`).
3. Add a card to `index.md` and, if relevant, a section to the matching
   page in `pages/`.

## Notes

- `projects/clustering-portfolio-post.html` is a large exported notebook and is
  intentionally left as-is.
