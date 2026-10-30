# 5B Study Hub

A responsive class study portal backed by the separate 5B Study Hub Cloudflare API.

## Frontend
- Static HTML, CSS and JavaScript. No build step or package installation.
- Sign-in and open student registration.
- Teacher applications and owner requests enter the approval queue.
- Student dashboard, papers, worksheets, practice questions, assignments, discussions, announcements, games and class chat.
- Owner account management and approval screen.
- Bearer-token session stored in the browser's local storage.

## Backend
API: https://5b-study-api.lujinsg.workers.dev/api/v1

This frontend does not use Lupin Cloud. The API and D1 database are separate.

## Deploy with Cloudflare Pages
Create a Pages project named **5b-study-website** and connect this repository:
- Production branch: `main`
- Build command: leave blank
- Build output directory: `/`

The project name is intentional: the current API CORS allowlist accepts the `5b-study-website*.pages.dev` host pattern.

## Important
- Never put the owner bootstrap secret in this repository or frontend JavaScript.
- The first owner account must be created through the protected backend bootstrap process.
- Teacher and owner requests require approval from an existing owner.
- Google Drive and Google Docs links are opened directly; file contents are not uploaded to this site.
