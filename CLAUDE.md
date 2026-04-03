# AustinBoren.com

Personal portfolio site for Austin Boren — iOS developer.

## Stack

Pure HTML and CSS. No JavaScript framework, no build tools, no package manager. Everything lives in `index.html`.

## File Structure

```
index.html          — The entire site (HTML + inline CSS)
0O1A0886-2.jpg      — Profile photo source file
profile.jpg         — The name the site expects for the hero image (rename/copy from source)
.vscode/
  launch.json       — VS Code debug config
```

> Note: the HTML references `profile.jpg`, but the actual photo on disk is `0O1A0886-2.jpg`. They need to match for the image to display.

## Development

Live preview via the **Live Server** VS Code extension (`ritwickdey.liveserver`):
- Right-click `index.html` → "Open with Live Server", or click "Go Live" in the status bar
- Serves at `http://localhost:5500` and auto-reloads on save

No build step. Edit `index.html` directly and save.

## Deployment

Static site — deploy by uploading `index.html` and `profile.jpg` to the host. No compilation needed.
