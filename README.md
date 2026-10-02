# Abdullah Mushtaq — Academic Portfolio

Personal academic website built with [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme, hosted on GitHub Pages.

**Live site:** [abdullahmushtaq78.github.io](https://abdullahmushtaq78.github.io)

## Pages

| Page | Path |
|---|---|
| About, Career, News, Contact | `index.md` |
| Research | `_pages/research.md` |
| Publications | `_pages/publications.md` |
| Teaching | `_pages/teaching.md` |
| Services | `_pages/services.md` |
| Media & Awards | `_pages/media.md` |
| CV | `_pages/cv.md` |

## Structure

```
├── _config.yml          # site settings, author info, sidebar links
├── _data/navigation.yml # top nav links
├── _includes/
│   ├── head/custom.html              # favicon, fonts, icons, stylesheets, SEO data
│   ├── footer/custom.html            # publications script + current-page marker in the nav
│   └── publications-filter.html      # turns publications.md into a filterable list
├── _pages/              # site pages
├── assets/
│   ├── css/main.scss        # MM theme imports + fonts and colour variables
│   ├── css/components.scss  # design tokens, hero, sidebar, nav, publications, research, contact
│   ├── images/          # headshot, favicon, research figures (images/research/)
│   └── pdf/cv.pdf       # CV PDF
└── index.md             # homepage
```

## Updating content

- **New publication:** copy the template at the top of `_pages/publications.md` into the list (newest first, preprints last). `Type` (Journal, Conference, or Preprint) decides which filter button it appears under.
- **New news item:** add an `<li><strong>Date</strong> Text</li>` at the top of the News list in `index.md`; move the oldest visible item into the "Earlier news" block to keep the list short. Write dates as `5 Aug 2026` or `Aug 2026`.
- **Dated lists** (Career, Teaching, Services, Awards): start each item with the date in bold and end the list with `{: .dated}`; the date moves into the left margin.
- **Update CV:** replace `assets/pdf/cv.pdf`
- **Profile photo:** replace `assets/images/headshot.jpg` (square, head and shoulders)
- **Research page:** each project in `_pages/research.md` is a `<div class="project">` block; copy an existing one and put its figure in `assets/images/research/` (about 1400px wide)
- **Sidebar links:** edit `author.links` in `_config.yml`

## Design notes

- **Type:** Gentium Book Plus (reading text and headings) and Atkinson Hyperlegible Next (navigation, dates, captions, buttons), loaded from Google Fonts in `_includes/head/custom.html`.
- **Colour:** Tulane green `#255C4E` on white, with highlighter tints for the annotated research statement and venue marks. Tokens are at the top of `assets/css/components.scss`.
- **Landing page:** the opening sentence is marked up like an NLP entity annotation (`<mark class="ent ent--model">…<span class="ent__label">model</span></mark>`).
