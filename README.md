# ousatov-ua

GitHub Pages portfolio template based on the structure of
[academicpages](https://github.com/academicpages/academicpages.github.io).

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Open <http://127.0.0.1:4000/ousatov-ua/>.

## Content entry points

- `_data/profile.yml` — name, role, links, interests, metrics.
- `_data/experience.yml` — CV experience blocks.
- `_data/projects.yml` — project cards and CV project bullets.
- `_data/publications.yml` — publication list.
- `_data/talks.yml` — talks list.
- `_pages/*.md` — static sections.
- `_portfolio/`, `_publications/`, `_talks/`, `_teaching/` — optional detail pages.

## Deployment

The `.github/workflows/github-pages.yml` workflow builds Jekyll and deploys to
GitHub Pages on every push to `main`.
