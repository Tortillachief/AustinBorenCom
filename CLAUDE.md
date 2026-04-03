# AustinBoren.com

Personal portfolio site for Austin Boren — iOS developer.

## Stack

HTML, inline CSS, and minimal vanilla JS. No framework, no build tools, no package manager. Everything lives in `index.html`.

## File Structure

```
index.html          — The entire site (HTML + inline CSS + vanilla JS)
images/
  headshot.jpg      — Hero portrait photo
.vscode/
  launch.json       — VS Code debug config
```

## Development

Live preview via the **Live Server** VS Code extension (`ritwickdey.liveserver`):
- Right-click `index.html` → "Open with Live Server", or click "Go Live" in the status bar
- Serves at `http://localhost:5500` and auto-reloads on save

No build step. Edit `index.html` directly and save.

## Deployment

Static site — deploy `index.html` and the `images/` directory to the host. No compilation needed.
