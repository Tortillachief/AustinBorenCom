# AustinBoren.com

Personal portfolio site for Austin Boren — iOS developer.

## Stack

HTML, inline CSS, and minimal vanilla JS. No framework, no build tools, no package manager. Everything lives in `index.html`.

## File Structure

```
index.html          — Main portfolio page (HTML + inline CSS + vanilla JS)
images/             — App icons and headshot
dark-tower/         — Dark Tower Classic app page
deep/               — Deep app page
chromaguess/        — Chroma Guess app page
.github/
  workflows/
    static.yml      — GitHub Actions deployment workflow
.vscode/
  launch.json       — VS Code debug config
```

## Development

Live preview via the **Live Server** VS Code extension (`ritwickdey.liveserver`):
- Right-click `index.html` → "Open with Live Server", or click "Go Live" in the status bar
- Serves at `http://localhost:5500` and auto-reloads on save

No build step. Edit `index.html` directly and save.

## Deployment

Deployed via GitHub Actions to GitHub Pages on every push to `master`. The workflow is defined in `.github/workflows/static.yml`.

**Important:** The workflow explicitly lists each directory to copy into the build. When adding a new app page directory, you must add a corresponding `cp -r <dirname> _site/` line to the "Build site" step in `static.yml`, otherwise the directory will not be deployed and the live site will 404.
