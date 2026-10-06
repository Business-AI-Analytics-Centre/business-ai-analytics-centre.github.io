# Business AI and Analytics Centre

The site is a static Jekyll website with custom layouts and styling, built for GitHub Pages.

## Local preview

Install Ruby 3.3 and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll. GitHub Pages can build the site from the `main` branch and repository root; supported plugins are declared in `_config.yml`.

## Updating site content

- Edit the homepage in `index.md`; shared layouts are in `_layouts/` and site styling is in `assets/css/style.css`.
- Update topic content in `_pages/`.
- Add or update people in `_data/people.yml`. Leave unverified details blank; people are sorted by name within their group.
- Update homepage news cards in `_data/news.yml` and event cards in `_data/events.yml`.
- Add dated Markdown posts to `_posts/` for news articles.
- Replace the empty `centre_email` value in `_config.yml` only when an approved address is available.
