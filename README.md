# Health Insurance Guide

Arabic reader for the Health Insurance Authority guide: 127 pages of text with search, an index and bookmarks.

## What it does

- Shows the guide page by page, with an index and previous and next navigation.
- Searches with Fuse.js, with Arabic letters normalised (alef forms, teh marbuta, alef maksura, diacritics). `/` focuses the search, and the arrow keys move between pages and results.
- Keeps bookmarks, and copies a link to a page.
- Appearance settings: light or dark theme, Amiri or Cairo font, size, line spacing and alignment, Arabic or English interface.
- Shows reading time and word count for a page. 25 pages have a card layout for violations and penalties.
- Links to `protocols.pdf` (download), the previous version of the guide and an experimental page.

## What it does not do

- It is a reader. It has no editing, accounts or sync.
- The text is built into the page. It is not fetched or updated from a server.
- Bookmarks and appearance settings are kept in `localStorage` under `appSt_v7`.
- The previous version and the experimental page are separate sites that this page only links to.

## Network and install

Loads Fuse.js 7.0.0 from cdnjs and the fonts from Google Fonts. It makes no other requests until you follow a link. Not installable; no service worker.

## Built with

One HTML file, with no build step and no framework. Fuse.js 7.0.0 provides the search.

## Run locally

Open `index.html` in a browser, or serve the folder with any static file server.
