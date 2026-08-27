# CSS Lab — Visual Lesson Atlas

This repository contains the original CSS lesson examples plus a unified dashboard at `index.html`.

Serve the folder with a static web server before using the Code view or Playground, because the browser fetches each original lesson file on demand. The dashboard groups all 42 lesson pages by topic, provides lesson search, and loads the selected original HTML UI into the preview workspace when its button is pressed. The sidebar is compact on desktop and becomes a slide-out menu on smaller screens. The preview toolbar can switch between Desktop, Tablet (768 × 920), and Mobile (390 × 844) device sizes. Preview scrollbars are hidden for a cleaner device-frame appearance while scrolling remains available. Each lesson includes a short explanation, focus chips, Previous/Next controls, a Code view for the original HTML/CSS, and an image fallback for failed remote assets.

The **Playground** view extracts each lesson’s HTML and CSS into editable panels and renders the result live in a sandboxed frame. Syntax, example, full source, and playground snippets include copy buttons. Remote lesson images are cached, loaded lazily when they approach the preview viewport, and given a fallback state if they fail. `sitemap.xml`, `robots.txt`, canonical metadata, Open Graph tags, Twitter Card tags, and a custom `assets/og-image.png` support discovery and link sharing.

## Local preview

```bash
python3 -m http.server 4173
```

Then visit <http://127.0.0.1:4173/>.

The original lesson files remain in their existing category folders. The dashboard uses relative paths, so it also works when hosted as a static GitHub Pages site.
