# Fitness Life

Fitness club chain, Krasnodar — a Tilda landing page, exported as a static site.

**Live:** https://erix319.github.io/tilda-fitness-life/

## About

Multi-location site for a fitness chain — four clubs plus three partner venues, fifteen years in Krasnodar. A club picker routes to per-location pages, alongside group-training schedules, equipment and facility highlights, and a free guest-visit lead form.

Interface language is Russian.

## Stack

- **Tilda** — Zero Block layout, built from the platform's page builder
- **Static export** — plain HTML, CSS and JavaScript, no build step and no server
- Tilda's runtime bundle: grid, lazy-loading, forms, menu and animation modules

## Running locally

Any static file server works. From the repository root:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

Opening `index.html` straight off the filesystem mostly works too, but a
server is closer to how it is actually deployed.

## Layout

```
index.html   the page itself
assets/      32 files — styles, scripts, images and fonts
```

## Notes

- Archived from https://project12923395.tilda.ws/, then repackaged: the saved asset folder was renamed
  to `assets/` and every reference rewritten, so the paths survive being served
  over HTTP instead of only from a local disk.
- The club picker links to `/club1`–`/club4` on the original host; those sub-pages were not part of the saved export, so they will not resolve here.
- Third-party endpoints in the original markup are left untouched. Forms still
  post to Tilda's handler and analytics still call home, so anything submitted
  here goes wherever the original site pointed it — treat this as a display
  copy, not a working intake channel.
