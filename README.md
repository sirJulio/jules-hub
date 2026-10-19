# Jules Hub

Julio's online front door: a single page with two choices, the professional site and the project portal. Plain HTML and CSS, no JavaScript, no build step.

## Files

| File | What it does |
|---|---|
| `index.html` | The page: title and the two choices |
| `styles.css` | All styling, including light and dark themes |
| `docs/brief.md` | What the hub is for, decisions made and open questions |

## When a site goes live

Each choice is a `<div class="choice">` until its site is online. To make it a working link, follow the comment in `index.html`: turn the `<div>` into an `<a class="choice" href="https://...">`, then swap "Opening soon" for the Visit arrow. Commit and push, and the live site updates.

## Viewing it locally

Double-click `index.html` to open it in your browser.

## Publishing

Planned: Cloudflare Pages, connected to this repo. No build command; output directory `/`.
