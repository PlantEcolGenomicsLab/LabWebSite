# Lab of Plant Ecological Genomics website

Hugo site for the Lab of Plant Ecological Genomics (Biodiversity Research Center, Academia Sinica),
deployed to GitHub Pages by `.github/workflows/hugo.yaml` on every push to `main` and once a day.

## Where things live

| What | File |
|---|---|
| Lab name, tagline, intro, contact, "We're hiring" banner | `hugo.toml` → `[params]` |
| Top navigation | `hugo.toml` → `[menus]` |
| Research projects (one file each) | `content/research/*.md` |
| Research overview | `content/research/_index.md` |
| People | `data/people.yaml` (+ photos in `static/images/people/`) |
| Recruiting / Join us | `content/join.md` |
| News posts | `content/news/*.md` |
| Publications | synced automatically from [ShengKaiHsu/cv](https://github.com/ShengKaiHsu/cv) by `scripts/sync_cv.py` |
| Colours and layout | `assets/site.css` |

Placeholders waiting for real text are marked `TODO(PI)`.

### Adding a research project

Copy one of `content/research/*.md`. Front matter fields:

- `title`, `description`: shown on the card and the page header.
- `icon`: one of `globe`, `dna`, `spark`, `leaf`.
- `weight`: sort order (lower comes first).
- `keywords`: tags shown at the bottom of the page.
- `publications`: DOIs (as in the CV, e.g. `https://doi.org/...`) to list as related papers.

### Adding a news post

Create `content/news/YYYY-short-name.md` with `title`, `date` and an optional `description`.

## Local preview

```bash
python3 scripts/sync_cv.py
hugo server
```
