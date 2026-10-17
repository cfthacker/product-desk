# Product Desk

A personal notebook for a product lead: keep the bigger missions visible, organize ongoing projects and conversations, and leave a short note about where things stand\.

## Features

- Missions, projects, threads, and standalone deliverables\.
- Inline notes with a dated history\.
- People and linked documents at mission or project level\.
- Deadlines with date and time in America/New\_York\.
- Pins, a scratchpad, completion, follow\-ups, and a recoverable shelf\.
- Drag ordering within and across compatible groups, with keyboard and menu alternatives\.
- JSON export and import for backups\.

## Run locally

The application is plain HTML, CSS, and JavaScript\. It has no build step or package dependencies\.

From this directory, run:

```sh
python -m http.server 8000 --directory dist
```

Then open http://localhost:8000\. Any static web server can serve the contents of `dist/`\.

## Files

- `dist/index.html` — application shell\.
- `dist/style.css` — responsive styles\.
- `dist/app.js` — data model, migration, interface, and interactions\.

## Data and backups

Workspace data is saved in the current browser’s local storage under `product-desk-v2`\. The repository includes the initial work examples; notes and changes made inside the app are separate browser data and are not automatically committed to GitHub\.

Use **••• → Export backup** to save current workspace data, and **Import backup** to restore it\. Export from the existing hosted app and import into a new host when moving the app: different origins have separate browser storage\.

There is no server, shared database, automatic cross\-device sync, or calendar notification integration in this version\. File links retain the permissions of their original hosts\.

## Hosting

Serve the contents of `dist/` from a static web host\. Copying this source does not change the existing private Product Desk deployment\.
