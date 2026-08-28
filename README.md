# leseixas.github.io

Academic site of Leandro Seixas, built with [Jekyll](https://jekyllrb.com/) on the
[academicpages](https://github.com/academicpages/academicpages.github.io) template and
published with GitHub Pages at <https://leseixas.github.io>.

It mirrors the section structure of <https://seixas.dev>: Home, CV, Portfolio,
Publications and Contact.

## Running it locally

```bash
bundle install
bundle exec jekyll serve --livereload
```

The site is then at <http://localhost:4000>. There is also a container setup:

```bash
docker-compose up
```

## Where things live

| Path | What it holds |
|---|---|
| `_pages/` | Every page. `about.md` is the home page (`permalink: /`). |
| `_config.yml` | Site settings, author profile and the links in the sidebar. |
| `_data/navigation.yml` | The masthead menu. |
| `_sass/layout/_custom.scss` | Cards, stat tiles, CV entries and publication list styles. |
| `files/` | Publication PDFs, named `001.pdf` … `030.pdf`. |
| `bibtex/` | One BibTeX record per publication, matching the PDF numbering. |
| `images/` | Avatar, favicons and social preview image. |

### Adding a publication

1. Drop the PDF in `files/` and the BibTeX record in `bibtex/`, using the next
   number in the sequence. **The two numbers must refer to the same paper** — the
   page links `/files/NNN.pdf` and `/bibtex/NNN.bib` side by side.
2. Add a `<div class="pub">` block to `_pages/publications.md` under the right
   year, with the DOI, the PDF link and the BibTeX link.
3. Bump the counts in the `stat-grid` at the top of that page.

## Notes

- The former `/experience/`, `/education/`, `/teaching/`, `/funding/`, `/talks/`
  and `/people/` pages are now sections of `/cv/` and redirect there via
  `jekyll-redirect-from`.
- This repository lives inside a Dropbox folder. Dropbox can turn a rename into a
  "conflicted copy" mid-operation; check `git status` after moving files around.

## License

Content © Leandro Seixas. Template code under the [MIT License](LICENSE).
