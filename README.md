# Business AI and Analytics Centre

The site is a static Jekyll website using the Minimal Mistakes theme and GitHub Pages-supported plugins.

## Local preview

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll. GitHub Pages can build the site from the `main` branch and repository root; the remote theme and plugins are declared in `_config.yml`.

## Updating site content

- Edit the homepage in `index.md` and the topic pages in `_pages/`.
- Add or update people in `_data/people.yml`. Leave unverified details blank; people are sorted by name within their group.
- Update homepage news cards in `_data/news.yml` and event cards in `_data/events.yml`.
- Add dated Markdown posts to `_posts/` for news articles.
- Replace the empty `centre_email` value in `_config.yml` only when an approved address is available.
