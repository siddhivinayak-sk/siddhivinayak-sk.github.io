## Sandeep Kumar's Profile Site

A personal professional profile and portfolio built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/). The site uses the Cayman theme with custom styling and shared page navigation.

### Site Pages

- **Home** (`index.md`): Introduction, highlights, selected work, and contact links.
- **Profile** (`profile.md`): Experience, focus areas, industries, and recognition.
- **Projects** (`projects.md`): Selected open-source solutions.
- **Writing** (`writing.md`): Technical articles grouped by topic.
- **Credentials** (`credentials.md`): Education and certifications.

Shared navigation is maintained in `_includes/site-nav.html`. Site title, description, and theme settings are in `_config.yml`; custom styling is in `assets/css/style.scss`.

### Preview Locally

Install Ruby, Bundler, and the GitHub Pages gem, then run Jekyll from the repository root:

```sh
gem install bundler
gem install github-pages
jekyll serve
```

Open the local URL printed by Jekyll, typically `http://localhost:4000`.

### Publish

GitHub Pages builds and publishes the site from the repository's configured Pages source when changes are pushed. To check or change the source, open the repository's **Settings → Pages**.

Edit the Markdown pages to maintain profile content. Keep the navigation destinations in `_includes/site-nav.html` aligned with page permalinks.
