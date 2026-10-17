# AO3 Bookmark Tracker

A single-file web app for tracking stats from your AO3 bookmarks over time. No build step, no backend.

## Features
- Table of works: link, title, author, summary, word count, likes (kudos), notes, read date, plus fandom, language, rating, tags, status, chapters, hits, bookmarks count, comments count
- Bulk import from a spreadsheet: paste cells, or upload `.csv`, `.tsv`, or `.xlsx`
- Dated stat snapshots: re-importing or editing a work logs changes in likes, words, hits, bookmarks, and comments
- Date filters (default: year to date), search, sort, monthly words chart, collapsible insights (fandoms, tags, authors, pace, length), CSV export

## Usage
Open `index.html` in a browser, or enable GitHub Pages (Settings → Pages → deploy from `main`, root).

Matching works are identified by AO3 link (`/works/<id>`), falling back to title + author.

## Data
Stored in your browser's `localStorage` (private per browser). Use **Export CSV** for backups.

## Notes
The `.xlsx` reader loads SheetJS from cdnjs; CSV and paste import work offline.
