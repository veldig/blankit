# BlankIt

**Insert a blank page after every page in a PDF — perfect for double-sided printing.**

Drop in a PDF, click one button, get a new PDF back instantly. No upload, no sign-up, no server. Everything runs in your browser using [pdf-lib](https://pdf-lib.js.org).

## What it does

Takes any PDF and inserts a blank page after every existing page, doubling the page count. Blank pages match the exact dimensions of the original page. Great for printing documents double-sided when you want each "real" page on its own sheet.

## How to use

1. Open `index.html` in any modern browser (or visit the hosted version)
2. Drag and drop a PDF, or click to browse
3. Click **Add Blank Pages**
4. The processed PDF downloads automatically

## Deploy to Netlify

Just drag `index.html` onto [app.netlify.com/drop](https://app.netlify.com/drop) — no build step required. Or connect this GitHub repo in the Netlify dashboard for automatic deploys on every push.

## Tech

- Single HTML file, zero dependencies to install
- [pdf-lib](https://pdf-lib.js.org) loaded from CDN for PDF manipulation
- Works with large PDFs — yields to the browser event loop every 20 pages
