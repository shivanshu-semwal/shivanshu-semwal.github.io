# Shivanshu Semwal

Personal portfolio and project index, published with GitHub Pages at
<https://shivanshu-semwal.github.io>.

## Local development

The repository pins Ruby 3.4.13 in `mise.toml` and the `Gemfile`.

```sh
mise install
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll. To build the site without serving it:

```sh
bundle exec jekyll build
```

GitHub Pages publishes the site from this repository using the `github-pages`
gem and Jekyll configuration in the root. The build output is written to
`_site/`, which is ignored by Git.

## Site content

- `index.html` contains the homepage introduction; `_layouts/home.html` adds
  the featured projects section.
- `_data/projects.yml` is the project list. Add or edit entries there with a
  `title`, `description`, `url`, and `featured` boolean; `stack` is optional.
  Set `featured: true` to show a project on the homepage; all entries appear
  on `/projects/`. List order is display order.
- `projects.md` and `about.md` provide the projects and about pages.
- `assets/css/style.scss` contains the site styles, and `assets/images/`
  contains the homepage landscape images.
- The header offers system, light, and dark theme modes; a selected mode is
  saved in browser local storage.

Jekyll site settings, including the title, description, URL, and SEO plugin,
are in `_config.yml`.
