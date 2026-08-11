# pixelmesh.website

The public site for [pixelmesh.live](https://pixelmesh.live) - the audience-pixels system
that turns a room full of phones into one screen.

The system itself lives in a separate repo; this one is only the website.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | The whole page. Styles and scripts are inline. |
| `public/` | Images, video, fonts, stats. The URL structure matches the old FastAPI hosting, so shared links still resolve. |
| `telemetry/<show>/index.html` | Per-show telemetry write-ups (e.g. `/telemetry/london-2026-06`). |

- Fonts are self-hosted in `public/fonts/` - there are no third-party requests.
- The hero loop, detection clip, poster and `og-image.jpg` are cut from real show footage.

## Deploying

Static site on DigitalOcean App Platform, served from the repo root. **Every push to `main`
deploys it**, so pushes are releases.

## Copy rules

- **pixelmesh is always lowercase**, including at the start of a sentence.
- No em dashes in site copy.

## Local preview

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.
