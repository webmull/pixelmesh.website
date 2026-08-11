# pixelmesh.website — Claude Instructions

## Never push without permission

Commit freely, but **never `git push` unless Adam has explicitly asked for or
approved the push** in the current conversation. `main` deploys the live site
on every push, so an unasked push is a deploy.

## Brand name is always lowercase

The product is written "pixelmesh" — never "PixelMesh", "Pixelmesh", or
"PIXELMESH" — in all copy, docs, headings, commit messages and UI strings,
including at the start of sentences.

## No em dashes in site copy

Use periods, colons or middots instead.

## What lives here

Only the public website. `index.html` is the whole page (styles and scripts
inline); assets sit under `public/` so the URL structure matches the old
FastAPI hosting and existing shared links still resolve. The pixelmesh system
itself is in the separate `pixelmesh` repo.
