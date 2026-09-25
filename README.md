# Home Inspection Companion

A static, mobile-first field app for room-by-room inspection notes, private photo evidence, repair follow-up, furniture decisions and printable reports.

## Live app

https://mushrath007.github.io/2700-dover-inspection-companion/

## Privacy model

- The website and reference photos are public.
- Entered inspection notes are saved in localStorage and added inspection photos are stored in the browser's IndexedDB database.
- Added photos are resized, re-encoded and stripped of embedded camera metadata before storage.
- The app has no analytics, account system, cloud database or note/photo-upload endpoint.
- JSON export/import includes notes and stored photos for durable backup and manual transfer between devices.
- Clearing browser/site data can erase notes that were not exported.

## Included

- Mobile inspection dashboard and quick feedback log
- Eleven detailed inspection areas
- Private camera/photo capture organized by inspection area
- Offline IndexedDB photo storage with download, deletion and backup/restore
- Seller-furniture decision worksheet
- 39-photo annotated visual assessment
- 18-page printable notebook and PDF
- Offline app shell and on-demand photo caching

## Local preview

Serve this directory with any local static server, then open the printed URL:

    python3 -m http.server 4173

## Deployment

The GitHub Actions workflow publishes the repository root to GitHub Pages.
