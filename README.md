# Chris Wang — Personal Academic Homepage

This repository contains the source code for [Chris Wang's personal academic homepage](https://kangw0916.github.io/), built with Jekyll and deployed through GitHub Pages.

## Pages

| Page | Route | Content |
|---|---|---|
| About Me | `/` | Biography, research interests, education experience, news and updates |
| Publications | `/publications/` | Publication list and paper cover images |

## Local development

Requires Ruby 3.3 and Bundler.

```bash
bundle install
bundle exec jekyll serve --livereload
# http://127.0.0.1:4000
```

Edit the Markdown files, then push to `main` for GitHub Pages to rebuild the site.

## Project structure

```text
.
├── _config.yml        # Site title, owner information and navigation
├── _includes/         # Shared head, footer and scripts
├── _layouts/          # Main page layout and responsive header
├── assets/             # CSS, JavaScript and fonts
├── images/             # Current photos, university emblems and paper covers
├── index.md            # About Me page
└── publications.md    # Publications page
```

## Customization

| What | Where |
|---|---|
| Name, avatar and social links | `_config.yml` |
| Navigation | `_config.yml` |
| Biography, news and education | `index.md` |
| Publications | `publications.md` |
| Photos and paper covers | `images/` |
| Colors and layout styles | `assets/css/main.css` |

## License

Code is released under the [MIT License](LICENSE). Site content, photos and publication material are © Chris Wang.
