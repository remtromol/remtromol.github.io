# My Art Portfolio Site Using Jekyll Workflow

This repository was converted from static HTML pages into a Jekyll-powered site without changing the visual design.

## Files and structure

- `home.md` → renders `/home`
- `projects.md` → renders `/projects`
- `about.md` → renders `/about`
- `_layouts/default.html` → shared page shell
- `_includes/sidebar.html` → sidebar navigation and social links
- `_includes/background.html` → background wrapper image
- `_includes/scripts.html` → carousel/lightbox scripts
- `_portfolio/*.md` → portfolio project data

## Adding a new portfolio item

1. Create a new file in `_portfolio/`, for example `_portfolio/new-project.md`
2. Add front matter like this:

```yaml
---
title: "Project Name"
tag: "Project Tag"
description: "Short description"
date: 2026-07-31
order: 4
images:
  - src: "https://example.com/image1.jpg"
    alt: "Image description"
    caption: "Caption text"
  - src: "/image/local-image.jpg"
    alt: "Local image description"
    caption: "Another caption"
---
```

3. Commit and push — Jekyll will render the new project automatically.

## Adding a blog post

1. (still on progess)



## Editing page content

- `home.md` controls the homepage content
- `projects.md` controls the projects page content and project list rendering
- `about.md` controls the info page content
- Shared layout changes go in `_layouts/default.html`
- Sidebar and background changes go in `_includes/sidebar.html` and `_includes/background.html`

## Preview locally

If you want to preview the site locally, install Jekyll and run:

```bash
gem install bundler jekyll
bundle exec jekyll serve --livereload
```

Then open `http://127.0.0.1:4000`.

## Thanks to

Jekyll - https://jekyllrb.com
