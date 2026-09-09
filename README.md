# gallery-dl — Instagram Post Archive Viewer

A single self-contained HTML file for browsing, organizing, and annotating a local Instagram post archive (from a `posts.json` export), running entirely offline in the browser — no server, no build step, no install.

## Usage

Open `postArchive.html` in Chrome or Edge. That's it.

## Features

- SQLite database (via sql.js / WebAssembly), with optional auto-save to a local `.sqlite` file (File System Access API)
- Per-post categories and free-form tags, with search, filtering, and sorting
- Free-text notes per post, with URLs auto-linked
- Image/video carousel with a full-size lightbox viewer
- Import/export posts as JSON, carrying category/tag/note data along with them
- Tools to find orphaned media files and re-sync the media index against disk
- Active/Hidden post views, with hide/restore/permanent-delete controls

## Requirements

Chrome or Edge recommended — the File System Access API (used for auto-saving the database and for the media-cleanup tools) isn't available in Firefox/Safari.

## Repository layout

- `postArchive.html` — latest version, ready to use
- `Archive/vX.x/` — snapshots of previous versions
