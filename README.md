# Fitness Life

Fitness club chain, Krasnodar — a Tilda landing page.

**Live:** https://pafuluofu-dev.github.io/tilda-fitness-life/

## About

Multi-location site for a fitness chain — four clubs plus three partner venues, fifteen years in Krasnodar. A club picker routes to per-location pages, alongside group-training schedules, equipment and facility highlights, and a free guest-visit lead form.

Interface language is Russian.

## Stack

- **Tilda** — Zero Block layout, built from the platform's page builder
- **Static site** — plain HTML, CSS and JavaScript, no build step and no server
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

- The club picker points at `/club1`–`/club4`, which are not part of this repository and will not resolve.
