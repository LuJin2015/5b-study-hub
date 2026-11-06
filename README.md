# 5B Study Hub

A responsive class study portal backed by the separate 5B Study Hub Cloudflare API.

## Frontend structure

- `index.html` is the dashboard.
- Each section has its own root-level folder and `index.html`, so URLs stay clean:
  - `/library/`
  - `/worksheets/`
  - `/practice/`
  - `/assignments/`
  - `/discussions/`
  - `/announcements/`
  - `/games/`
  - `/chat/`
  - `/people/`
- Shared files live in `assets/css/`, `assets/js/`, and `assets/images/`.
- No build step or package installation is needed.

## Backend

API: https://5b-study-api.lujinsg.workers.dev/api/v1

The API and D1 database are separate from Lupin Cloud.

## Publish with GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. GitHub Pages publishes the site at:

   https://lujin2015.github.io/5b-study-hub/

## Important

- The backend must allow the GitHub Pages origin `https://lujin2015.github.io` in its CORS policy.
- Never put the owner bootstrap secret in this repository or frontend JavaScript.
- Teacher and owner requests require approval from an existing owner.
- Google Drive and Google Docs links are opened directly; files are not uploaded to this site.
