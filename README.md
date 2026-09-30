# ucchwas.github.io

Personal website of Ucchwas Talukder Utsha, served by GitHub Pages from the `main` branch.
It is a small Jekyll site with no theme and no JavaScript.

## Updating content

Everything that changes regularly lives in `_data/`:

| File | Contents |
| --- | --- |
| `profile.yml` | Name, role, email, profile links, photo, and resume path |
| `news.yml` | Dated news items, newest first (the home page shows the first five) |
| `publications.yml` | All publications; `selected: true` also lists one on the home page |
| `projects.yml` | Projects; `home: true` also lists one under "Selected work" |
| `experience.yml` | Positions, each with one to three highlights |
| `education.yml`, `skills.yml` | Degrees and skill groups |

The bio paragraphs are in `index.html`. To update the resume, replace
`assets/pdfs/Ucchwas_Talukder.pdf`; the link stays the same.

## Structure

- `_layouts/default.html`: page shell (head, header, main, footer)
- `_includes/`: head metadata, structured data, header, footer, icons, and the publication and project entries
- `index.html`, `publications.html`, `projects.html`, `404.html`: the pages
- `assets/css/main.css`: all styles. It is plain CSS with no front matter, so Jekyll copies it as is.
- `assets/fonts/`: IBM Plex Sans and IBM Plex Mono subsets (SIL Open Font License, see `OFL.txt`)
- `assets/img/`: profile photo and social preview image

The old `/about/`, `/research/`, and `/achievements/` URLs redirect to the home page.

## Local preview

With Ruby 3 and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>. The `github-pages` gem pins the same Jekyll version and plugins
that GitHub Pages uses.
