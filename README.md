# 5B Study Hub

A responsive class study portal backed by the separate 5B Study Hub Cloudflare API.

## Frontend
- Static HTML, CSS and JavaScript. No build step or package installation.
- Student registration and sign-in.
- Teacher applications and owner requests enter an approval queue.
- Student dashboard, papers, worksheets, practice questions, assignments, discussions, announcements, games and class chat.
- Owner account management and approval screen.

## Backend
API: https://5b-study-api.lujinsg.workers.dev/api/v1

The API and D1 database are separate from Lupin Cloud.

## Publish with GitHub Pages
1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. GitHub Pages will publish the site at:

   https://lujin2015.github.io/5b-study-hub/

No build command is needed. The site is plain static HTML/CSS/JavaScript.

## Important
- The backend must allow the GitHub Pages origin `https://lujin2015.github.io` in its CORS policy.
- Never put the owner bootstrap secret in this repository or frontend JavaScript.
- The first owner account must be created through the protected backend bootstrap process.
- Teacher and owner requests require approval from an existing owner.
- Google Drive and Google Docs links are opened directly; files are not uploaded to this site.
