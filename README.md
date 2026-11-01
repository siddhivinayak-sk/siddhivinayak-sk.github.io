## Sandeep Kumar's Profile Site

A personal professional profile and portfolio built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/). The site uses the Cayman theme with custom styling and shared page navigation.

### Site Pages

- **Home** (`index.md`): Introduction, highlights, selected work, and contact links.
- **Profile** (`profile.md`): Experience, focus areas, industries, and recognition.
- **Projects** (`projects.md`): Categorized open-source project cards linking to GitHub.
- **Writing** (`writing.md`): Technical article cards grouped by topic and linking to Medium.
- **Credentials** (`credentials.md`): Education and certifications.

Shared navigation is maintained in `_includes/site-nav.html`. Site title, description, and theme settings are in `_config.yml`; custom styling is in `assets/css/style.scss`.

### Maintain the showcase

- Edit `_data/projects.yml` to add or update project names, repository names, categories, technologies, and descriptions. Set `featured: true` to include a project on the home page.
- Edit `_data/articles.yml` to add or update article titles, Medium URL slugs, categories, and descriptions. Set `featured: true` to include an article on the home page.
- Categories and item counts are generated from these lists. Shared card templates in `_includes/project-grid.html` and `_includes/article-grid.html` keep the home page and catalogs consistent.
- The lists are curated, not fetched in visitors' browsers. Project metadata was checked against public GitHub repositories; additional article links were sourced from the [Medium RSS feed](https://siddhivinayak-sk.medium.com/feed). Review the lists when publishing new work.
- Set `buymeacoffee_url` in `_config.yml` to change the support destination. `_includes/coffee-support.html` provides the shared support panel on Home, Projects, and Writing; the navigation also links to it. This is a plain link, with no third-party donation widget or tracking script.

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
