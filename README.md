# darkhorseftc.github.io

Team website for DarkHorse Robotics — custom Jekyll theme, built natively by
GitHub Pages on every push to `main`. Live at https://darkhorseftc.github.io

## Coach's guide

**Add a blog post:** create `_posts/YYYY-MM-DD-short-title.md`:

```markdown
---
title: "League Meet 0 recap"
---

Markdown body here.
```

**Add a portfolio entry:** same idea in `_portfolio/` (see the template entry there).

**Change the contact email:** one line in `_config.yml` (`email:`) — every
mailto button on the site follows it.

**Images:** drop files in `assets/img/`, reference as `/assets/img/name.jpg`.

## Hidden until ready

`/blog/` and `/portfolio/` render but are not linked from the homepage nav.
To go public with them, add to `_includes/nav.html`:

```html
<li><a href="/blog/">Log</a></li>
<li><a href="/portfolio/">Portfolio</a></li>
```

## Structure

- `index.html` — the single-page homepage (hero, season, schedule, team, sponsors)
- `_includes/` — topbar, nav, footer, head shared by every page
- `_layouts/` — `shell` (page frame), `post`, `portfolio-entry`
- `assets/css/main.css` — the whole theme: blue grounds, honey ink, Fredoka + Jost (both SIL OFL, self-hosted in `assets/fonts/`)
