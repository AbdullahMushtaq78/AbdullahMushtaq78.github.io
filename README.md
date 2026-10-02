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
│   ├── footer/custom.html            # loads the publications script
│   └── publications-filter.html      # turns publications.md into filterable cards
├── _pages/              # site pages
├── assets/
│   ├── css/main.scss        # MM theme imports + small overrides
│   ├── css/components.scss  # publication cards, research page, contact block, avatar
│   ├── images/          # headshot, favicon, research figures (images/research/)
│   └── pdf/cv.pdf       # CV PDF
└── index.md             # homepage
```

## Updating content

- **New publication:** copy the template at the top of `_pages/publications.md` into the list (newest first, preprints last). `Type` (Journal, Conference, or Preprint) decides which filter button it appears under.
- **New news item:** add a `<li>` in the news box in `index.md`
- **Update CV:** replace `assets/pdf/cv.pdf`
- **Profile photo:** replace `assets/images/headshot.jpg` (square, head and shoulders)
- **Research page:** each project in `_pages/research.md` is a `research-card` block; copy an existing one and put its figure in `assets/images/research/` (about 1400px wide)
- **Sidebar links:** edit `author.links` in `_config.yml`
