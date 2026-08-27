# CSS Lab — Visual Lesson Atlas

This repository contains the original CSS lesson examples plus a unified dashboard at `index.html`.

Open `index.html` directly in a browser, or serve the folder with any static web server. The dashboard groups all 42 lesson pages by topic, provides lesson search, and loads the selected original HTML UI into the preview workspace when its button is pressed.

## Local preview

```bash
python3 -m http.server 4173
```

Then visit <http://127.0.0.1:4173/>.

The original lesson files remain in their existing category folders. The dashboard uses relative paths, so it also works when hosted as a static GitHub Pages site.
