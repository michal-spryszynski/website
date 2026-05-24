# michal.spryszynski.pl

Simple personal website for Michał Spryszyński.

## Project info

- Deployment: static files served via Nginx on a VPS
- URL: https://michal.spryszynski.pl
- Stack: plain HTML + CSS, no frameworks, no build step

## Structure

Keep it as flat as possible:
index.html
style.css
No subdirectories unless absolutely necessary.

## Rules

- No JavaScript unless strictly needed
- No external dependencies, no CDNs
- Mobile-friendly, but keep CSS minimal
- No build tools, no npm, no bundlers

## Deployment

On every push to `main`, GitHub Actions rsyncs files to `/var/www/michal` on the VPS.
Do not add files that shouldn't be deployed publicly.