# Archive reconstruction policy

1. Query Wayback CDX for `mollypiercedesign.com/*`.
2. Group captures by normalized URL path.
3. Select the newest successful `text/html` capture for each page.
4. For the homepage and core navigation pages, prefer the newest common capture timestamp.
5. Backfill only missing pages and assets from older captures.
6. Save every recovered source URL in a migration manifest.
7. Convert repeated chrome into Astro components.
8. Preserve legacy routes where practical.
