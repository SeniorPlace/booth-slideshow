# Senior Place Booth Slideshow

A self-contained [impress.js](https://github.com/impress/impress.js) presentation for running at a convention booth. It starts playing on its own, advances every 9 seconds, and loops forever. Every screenshot is the real product (a demo tenant, "Rainier Senior Placement").

## Get it on a booth device

No account or credentials needed — the repo is public.

- **Just play it (device is online):** open
  **<https://seniorplace.github.io/booth-slideshow/>**
  and go full-screen (F11, or Add to Home Screen on an iPad).
- **Download one file (works offline afterward):**
  **<https://github.com/SeniorPlace/booth-slideshow/releases/latest/download/booth-slideshow.zip>**
  Unzip it and open `index.html` in any browser. That's the whole install.

The zip is repackaged automatically on every push to `master`, so that link always serves the newest version.

## At the booth

- It runs hands-off: auto-advance, infinite loop, cursor hides itself, and it asks the browser to keep the screen awake.
- Tap / click / arrow keys let you drive it manually during a conversation; auto-play resumes afterward.
- `Esc` shows the zoomed-out overview of the whole story.

## Editing

- Slides live in `index.html` (one `div.step` each; positions via `data-x`/`data-y`/`data-rotate`).
- Screenshots live in `img/` — regenerate from a local demo tenant and drop in replacements with the same filenames.
- Styling in `css/booth.css`; the auto-advance interval is `data-autoplay` on `#impress`.
