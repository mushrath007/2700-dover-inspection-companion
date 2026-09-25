# Home Inspection Companion

A static, mobile-first field app for room-by-room inspection notes, repair follow-up, furniture decisions and printable reports.

## Privacy model

- The website and reference photos are public.
- Entered inspection notes are saved only in the visitor's browser with localStorage.
- The app has no analytics, account system, database or note-upload endpoint.
- JSON export/import provides a durable backup and manual transfer between devices.
- Clearing browser/site data can erase notes that were not exported.

## Included

- Mobile inspection dashboard and quick feedback log
- Eleven detailed inspection areas
- Seller-furniture decision worksheet
- 39-photo annotated visual assessment
- 18-page printable notebook and PDF
- Offline app shell and on-demand photo caching

## Local preview

Serve this directory with any local static server, then open the printed URL:

    python3 -m http.server 4173

## Deployment

The GitHub Actions workflow publishes the repository root to GitHub Pages.
