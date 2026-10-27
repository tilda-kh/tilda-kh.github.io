# Personal site

A small Hugo site with no external theme. Everything lives in this folder.

## Run it locally
1. Install Hugo (extended): https://gohugo.io/installation/
2. In this folder, run `hugo server` (add `-D` to also show drafts)
3. Open http://localhost:1313

## Fill it in
- **Home page:** `content/_index.md`
- **Your photo:** put it in `static/img/` (e.g. `static/img/me.jpg`), then change the `photo` line in
  `content/_index.md` to `src="/img/me.jpg"`, with a description in `alt` and an optional `caption`.
  The same `{{< photo ... >}}` line works in any page or post.
- **Pages:** `content/now.md`, `content/academic.md`
- **New posts or projects:** `hugo new blog/title.md` or `hugo new projects/title.md`, then set `draft: false`
- **Footer links and site name:** `hugo.toml`
- **Navigation:** the `[menus]` section of `hugo.toml`
- **Colours and font:** the variables at the top of `assets/css/main.css`

## Publish it
Run `hugo` to build into `public/`. Netlify, Cloudflare Pages and GitHub Pages host Hugo sites for free;
use the build command `hugo` and the output directory `public`.
