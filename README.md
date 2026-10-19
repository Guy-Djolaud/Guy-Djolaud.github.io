# Guy-Arnold Djolaud – personal academic website

Source of <https://guy-djolaud.github.io>, built with Jekyll on GitHub Pages
(based on the [AcademicPages](https://github.com/academicpages/academicpages.github.io) template).

## Where things live

| What | Where |
| --- | --- |
| Home page text | `_pages/about.md` |
| Sidebar (name, photo, links) | `author:` section of `_config.yml` |
| Top menu | `_data/navigation.yml` |
| Papers (Research page) | `_publications/*.md` – `category:` is `manuscripts`, `conferences` or `books` |
| Talks | `_talks/*.md` |
| PDFs (CV, papers, slides) | `files/` – served at `/files/<name>.pdf` |
| Images | `images/` |

## Adding a paper

Create `_publications/<slug>.md`:

```yaml
---
title: "Paper title"
collection: publications
category: manuscripts
permalink: /publications/<slug>
excerpt: 'with [Coauthor](https://example.com)'
date: 2026-01-31
paperurl: '/files/<paper>.pdf'
slidesurl: '/files/<slides>.pdf'
---
Abstract.
```

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

or `docker compose up`, then open <http://localhost:4000>.
