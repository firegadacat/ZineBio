# ZineBio ✍️
> A zero-setup Markdown-driven personal bio builder that runs entirely in your browser.

Write in Markdown. Style with live CSS. Script with live JS. Publish in one click — all in a **single HTML file**, no backend, no build step.

![ZineBio Preview](https://img.shields.io/badge/version-1.1.0-brightgreen?style=flat-square) ![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square) ![No dependencies](https://img.shields.io/badge/dependencies-none-orange?style=flat-square)

---

## ✨ Features

- 📝 **Live Markdown editor** — split-panel with real-time preview
- 🎨 **5 built-in themes** — Default Light, Dark Terminal, Warm Paper, Bold Editorial, Soft Pastel
- 🖌️ **Custom theme builder** — pick your own background, text, heading, accent, and card colors with a color picker
- 💅 **Live CSS editor** — write and apply your own custom CSS on the fly
- ⚡ **Live JS editor** — write custom scripts (e.g. for analytics, custom widgets, or interactive tags) that run inside a safe sandbox in the live preview panel and bundle directly into your export
- 🎴 **Interactive Card Grids** — divide your page sections into side-by-side grids of link cards (`.grid-2`, `.grid-3`, `.link-card`) that responsively stack on mobile screens
- 📦 **CSS Snippet library** — one-click presets for dark mode overrides, custom fonts, badges, spoiler text, card sections, frosted glass cards, and more
- 🗂️ **Section Manager** — drag-and-drop sidebar chip lists to reorder your bio sections
- 📱 **Mobile Responsive layout** — responsive headers, side-scrolling custom swatches, touch-optimized toolbars, table layout overflow control, and floating overlay drawer managers that adjust flawlessly on phone displays
- 🔒 **Keyboard-Safe Edit Panels** — editors scale to 100% viewport heights on mobile to avoid virtual keyboard overlapping and screen squishing
- 💾 **Auto-save** — everything saved to `localStorage`, survives refresh
- 📤 **Export** — export a clean standalone static HTML bio page, or save/load raw `.md` files
- ⌨️ **Toolbar shortcuts** — quick-insert buttons for bold, italic, links, images, code blocks, tables, badges, grids, widgets, and more
- 🔍 **Theme-Aware Syntax highlighting** — code block highlights inherit colors based on the active theme (e.g. Dracula aesthetic on Terminal, Earthy forest tones on Warm Paper) powered by highlight.js
- 📴 **Works offline** — after first load, CDN assets are cached

---

## 🚀 Getting Started

No install. No setup. Just open the file.

```bash
# Clone the repo
git clone https://github.com/your-username/zinebio.git

# Open in browser
start zinebio/index.html   # Windows
open zinebio/index.html    # macOS
xdg-open zinebio/index.html # Linux
```

Or just [download the HTML file](./index.html) directly and open it in any modern browser.

---

## 🖥️ How to Use

### Edit Mode
1. **Write your bio** in the Markdown panel on the left
2. See the **live preview** update on the right instantly
3. Switch themes using the **theme dropdown** in the top bar
4. Customize colors with **🎨 Custom...** theme option
5. Open the **CSS** and **JS** tabs to write custom code or apply snippets

### View Mode
- Click the **View Bio** pill button (bottom right) to toggle to a clean, fullscreen view of your bio

### Export
- **Export HTML** — generates a standalone, self-contained HTML bio page (no editor, just the beautiful bio + custom CSS + sanitized JS bundle)
- **Export .md** — saves your raw Markdown file
- **Import .md** — load an existing Markdown file

---

## 🎨 Themes & Syntax Highlights

ZineBio features full code block syntax highlights designed to match the palette of each theme:

| Theme | Colors | Syntax Palette |
|---|---|---|
| ✨ Default Light | Light paper & dots | Clean github-light (reds, dark blues, slate greys) |
| 📟 Dark Terminal | Emerald & pitch black | Neon cyberpunk (pinks, bright yellows, cyan, purple) |
| 📜 Warm Paper | Ruled warm parchment | Earthy forest (warm reds, leaf greens, warm greys) |
| 📰 Bold Editorial | High-contrast grid | High impact (roses, deep teal, purple, slate) |
| 🌸 Soft Pastel | Lilac circles & pastels | Muted soft pastels (sky blues, violets, soft fuchsias) |
| 🎨 Custom... | Fully customizable | Inherited style |

---

## 💅 CSS Snippets

Click the **CSS Snippets** dropdown in the CSS tab to instantly insert:

- 🌓 **Media Dark Mode Override** — auto dark mode via `prefers-color-scheme`
- 🎨 **Accent color override** — change the accent color globally
- 🔤 **Google Fonts @import** — swap in any Google Font
- 📏 **Centered narrow layout** — narrow 600px centered content column
- 📦 **Card-style sections** — box sections with hover shadows
- 🏷️ **Sleek gradient pill badges** — style `.badge` elements
- 🫣 **Spoiler text** — hover-to-reveal hidden text
- 🎴 **Translucent Frosted glass card styles** — custom transparent background and backdrop blurring for cards

---

## 🧩 Markdown Extensions

ZineBio supports standard Markdown plus some handy extras via HTML classes:

```html
<!-- Badge -->
<span class="badge">Open to Work</span>

<!-- Spoiler (hover to reveal) -->
<span class="spoiler">Hidden text here</span>

<!-- Side-by-side cards (2-column layout) -->
<div class="grid-2">
  <a href="https://github.com" class="link-card" target="_blank">
    <div class="card-icon">🐙</div>
    <div class="card-info">
      <div class="card-title">GitHub Profile</div>
      <div class="card-subtitle">github.com/username</div>
    </div>
    <div class="card-arrow">→</div>
  </a>

  <a href="https://x.com" class="link-card" target="_blank">
    <div class="card-icon">🐦</div>
    <div class="card-info">
      <div class="card-title">Twitter / X</div>
      <div class="card-subtitle">x.com/username</div>
    </div>
    <div class="card-arrow">→</div>
  </a>
</div>

<!-- Full-width Call-to-action widget card -->
<div class="link-card widget-card">
  <div class="card-icon">💬</div>
  <div class="card-info">
    <div class="card-title">Join Our Discord Community</div>
    <div class="card-subtitle">🟢 120 Online • 🟣 450 Members</div>
  </div>
  <a href="https://discord.gg/invite" class="widget-btn" target="_blank">Join Server →</a>
</div>
```

---

## 🗂️ Section Manager

The sidebar drawer lists all your `##` headings as draggable section cards.  
Drag them to reorder — the Markdown updates automatically.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| [marked.js](https://marked.js.org/) | Markdown → HTML rendering |
| [highlight.js](https://highlightjs.org/) | Syntax highlighting in code blocks |
| [Google Fonts](https://fonts.google.com/) | Typography |
| Vanilla HTML/CSS/JS | Everything else — zero frameworks |

---

## 📁 Project Structure

```
zinebio/
└── index.html   # The entire app — self-contained single file
```

---

## 📄 License

MIT — do whatever you want with it. Credit appreciated but not required. 🙂

---

<p align="center">Made with ☕ and too much CSS & JS</p>
