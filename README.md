# poulos.me

Personal website of Jason Poulos, built with [Jekyll](https://jekyllrb.com/) and served by GitHub Pages at <https://poulos.me> (see `CNAME`).

## Updating content

Almost everything lives in `_data/`; edit these files rather than the HTML:

| File | Controls |
|---|---|
| `_data/main_info.yaml` | Name, title, email, social links (LinkedIn, GitHub, Google Scholar, ORCID), site description for search/social previews, profile photo, Google Analytics 4 ID |
| `_data/news.yaml` | News items, newest first (`date`, `text`; text may contain HTML) |
| `_data/publications.yaml` | Publications; `selected: y` shows a paper under "Selected"; optional buttons: `paper_pdf`, `arxiv`, `code`, `website`, `blog`, `slides`, `poster`, `video`, `data`, `supplementary` |
| `_data/projects.yaml` | Projects; `selected: y` shows under "Selected"; optional buttons: `website`, `code`, `paper`, `blog` |
| `_data/experience.yaml` | Vitæ timeline; `category: "work"` renders on the left, `"school"` on the right |

The CV and resume PDFs are `assets/cv/jvp-vita.pdf` and `assets/cv/jvp-resume.pdf`; replace those files to update the links in the header and Vitæ section. Their LaTeX sources live outside this repository (`Dropbox/jvp-vita/`).

Page structure is in `index.html` (sections) and `_layouts/default.html` (head, header, navigation, footer). Custom styles are in `libs/custom/my_css.css`.

## Previewing locally

```
jekyll serve
```

then open <http://127.0.0.1:4000>.

## Publishing

Commit and push to `master`; GitHub Pages rebuilds and publishes the site automatically.

## Analytics

Analytics are off by default. To enable Google Analytics 4, set `ga4_measurement_id` (for example `G-XXXXXXXXXX`) in `_data/main_info.yaml`.

## Credits

- Design adapted from [Martin Saveski's website template](https://web.stanford.edu/~msaveski/).
- CSS: [Skeleton](http://getskeleton.com/), [Skeleton Tabs](https://github.com/nathancahill/skeleton-tabs)
- Icons: [Font Awesome](https://fontawesome.com/) (via cdnjs) and [Academicons](https://jpswalsh.github.io/academicons/)
- JavaScript: [jQuery](https://jquery.com/)
