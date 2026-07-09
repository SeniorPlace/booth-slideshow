# Senior Place Booth Slideshow

A self-contained [impress.js](https://github.com/impress/impress.js) presentation for running at a convention booth. Every screenshot is the real product (a local demo tenant, "Rainier Senior Placement").

## Running it

There is no build step and no network dependency — everything is local files.

- **Anywhere with a browser**: open `index.html`. That's it.
- **iPad / Chromebook at a booth**: either
  - serve the folder (`python3 -m http.server 8000`) from any machine on the booth network and open `http://<host>:8000` full-screen, or
  - put the folder on the device (Files app / Downloads) and open `index.html` in the browser, then Add to Home Screen / full-screen it.
- **GitHub Pages**: the repo is a static site — enable Pages on `main` and open the published URL on any device.

## Booth mode

The deck auto-advances every 9 seconds and loops forever — start it, go talk to people.

- Tap / click / spacebar / arrow keys advance manually (auto-play pauses while you drive, and resumes).
- Press `Esc` for the zoomed-out overview of the whole story.

## Editing

- Slides live in `index.html` (one `div.step` each; positions via `data-x`/`data-y`/`data-rotate`).
- Screenshots live in `img/` — regenerate them from a local demo tenant and drop replacements in with the same filenames.
- Styling in `css/booth.css`; auto-advance interval is `data-autoplay` on `#impress`.
