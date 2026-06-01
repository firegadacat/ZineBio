# ZineBio ✍️
> A zero-setup Markdown-driven personal bio builder that runs entirely in your browser.

Write in Markdown. Style with live CSS. Publish in one click — all in a **single HTML file**, no backend, no build step.

![ZineBio Preview](https://img.shields.io/badge/version-1.0.0-brightgreen?style=flat-square) ![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square) ![No dependencies](https://img.shields.io/badge/dependencies-none-orange?style=flat-square)

---

## ✨ Features

- 📝 **Live Markdown editor** — split-panel with real-time preview
- 🎨 **5 built-in themes** — Default Light, Dark Terminal, Warm Paper, Bold Editorial, Soft Pastel
- 🖌️ **Custom theme builder** — pick your own background, text, heading, accent, and card colors with a color picker
- 💅 **Live CSS editor** — write and apply your own custom CSS on the fly
- 📦 **CSS Snippet library** — one-click presets for dark mode, badges, spoiler text, card sections, and more
- 🗂️ **Section Manager** — drag-and-drop sidebar to reorder your bio sections
- 💾 **Auto-save** — everything saved to `localStorage`, survives refresh
- 📤 **Export** — export a clean standalone HTML bio page, or save/load `.md` files
- ⌨️ **Toolbar shortcuts** — quick-insert buttons for bold, italic, links, images, code blocks, tables, badges, and more
- 🔍 **Syntax highlighting** — code blocks powered by highlight.js
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
5. Open the **CSS tab** to write your own styles or insert snippets

### View Mode
- Click the **View** pill button (bottom right) to toggle to a clean, fullscreen view of your bio

### Export
- **Export HTML** — generates a standalone, self-contained bio page (no editor, just the beautiful bio)
- **Export .md** — saves your raw Markdown file
- **Import .md** — load an existing Markdown file

---

## 🎨 Themes

| Theme | Description |
|---|---|
| ✨ Default Light | Clean minimal light theme with dot texture |
| 📟 Dark Terminal | Dark green-on-black terminal aesthetic |
| 📜 Warm Paper | Warm parchment with ruled lines |
| 📰 Bold Editorial | High-contrast editorial with vibrant rose accent |
| 🌸 Soft Pastel | Soft lilac and purple pastels |
| 🎨 Custom... | Full color picker — make it yours |

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

---

## 🧩 Markdown Extensions

ZineBio supports standard Markdown plus some handy extras via HTML classes:

```html
<!-- Badge -->
<span class="badge">Open to Work</span>

<!-- Spoiler (hover to reveal) -->
<span class="spoiler">Hidden text here</span>
```

---

## 🗂️ Section Manager

The left sidebar lists all your `##` headings as draggable section cards.  
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

<p align="center">Made with ☕ and too much CSS</p>
