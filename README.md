# DR01D website

**Ilya Lisogor · Junior Full-stack Developer**

[Website](https://dr01d.info/) · [Projects](https://dr01d.info/projects) · [Telegram](https://t.me/DR01D_0)

A minimal, bilingual portfolio with IBM Plex Mono, an adaptive home layout,
20 project cards and small, responsive animations. HTML, CSS and JavaScript;
no framework, build step or container required.

## Features

- English by default, Russian translation and a saved language preference.
- A home screen fitted to the viewport and a scrollable project list.
- /projects navigation, browser history and a local-file hash fallback.
- Embedded avatar, favicon, fonts and SVG icons in one HTML file.
- Email copying with compact success feedback and a failure fallback.
- Staggered entrances, scroll reveals and animated arrows; reduced-motion support.
- Semantic headings, keyboard navigation and visible focus states.

## Open locally

Download index.html and open it in a browser. All interface assets are embedded.
Linked websites, repositories, the game demo and downloads require internet access.

For a simple HTTP preview:

```sh
python -m http.server 8080
```

Open http://localhost:8080. A production host must map /projects to this HTML
file (or an identical copy named projects.html). The browser sets the correct
page title and view from the path.

## Hosting

Production uses static files on nginx with HTTPS. The quiz demo and public
DiskMonitor EXE are separate hosted artifacts, not bundled into this repository.
Keep private project sources and service credentials out of the web root.

## Checks

HTML structure, project order/privacy, skills and JavaScript syntax were checked.
Node VM scenarios cover routing, language persistence, clipboard success/failure,
focus, project reveals and reduced motion. Browser rendering and the system
clipboard remain manual checks.

Typography: IBM Plex Mono (see FONT-LICENSE.txt).
Visual direction and the base icon set follow [jnngl.dev](https://jnngl.dev/).
