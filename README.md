# 🎨 Jellyfin Artwork Generator

A free, browser-based tool for creating custom artwork for your [Jellyfin](https://jellyfin.org) media server — posters, backdrops, banners, logos, and more. No sign-up, no install, no watermarks. Everything runs locally in your browser.

**[→ Open the Generator](https://loyalwolf.github.io/Jellyfin-Artwork-Generator)**

---

## ✨ Features

- **All Jellyfin image types** — Primary, Backdrop, Banner, Thumb, Logo, Clearart, Box, Disc, and custom dimensions
- **Live preview** — changes render instantly as you type or adjust settings
- **30 fonts** across 7 categories — Rounded & Friendly, Bold & Display, Sci-Fi & Tech, Elegant & Serif, Handwritten & Fun, Retro & Pixel, System
- **6 text styles** — Gradient, Solid, Outline, Shadow, Neon, Stamp
- **Text positioning** — 9-point anchor grid with X/Y offset sliders
- **Second text layer** — independent font, size, color, alignment and position (great for subtitles, years, episode labels)
- **Gradient presets** — 8 curated presets with full custom 3-stop gradient control and 4 direction options
- **Background image** — upload any photo with opacity, blur, brightness, contrast, saturation, blend mode, and color overlay controls
- **Background gradient** — 3-stop gradient background with 5 directions including radial
- **Pattern backgrounds** — 6 built-in patterns (Dots, Grid, Diagonal, Chevron, Crosshatch, Hexagons) with color, opacity and scale control
- **Texture overlays** — Grain, Scanlines, Halftone, Scratches with intensity and blend mode control
- **Duotone** — maps image shadows and highlights to two custom colors, with intensity control
- **Shape elements** — decorative lines, circles, rectangles, diamonds and triangles with fill/outline style, size, thickness, opacity and position
- **Vignette effect** — radial dark edge with intensity, spread, and color controls
- **Logo/overlay image** — upload a second image (e.g. network logo) with 9-point positioning, size, opacity, and padding
- **Corner badge** — preset labels (4K, HDR, HDR10, DV, DUBBED, SUBBED, EXTENDED, UNRATED, NEW) or fully custom text
- **Border options** — color, width, corner radius, and style (solid, gradient-matched, inset glow)
- **Presets** — save and load named settings, with export/import via JSON file for backup and cross-browser use
- **Undo/Redo** — Ctrl+Z / Ctrl+Y with 50-step history
- **Batch export** — export all selected Jellyfin image types at once, each at the correct dimensions
- **Zoom & pan** — scroll wheel to zoom the preview up to 400%, click and drag to pan
- **PNG export** — full resolution with or without background (transparent export ideal for Logo and Clearart)
- **Auto font sizing** — text scales automatically to fill the canvas, or set a fixed size manually
- **No internet required** — works fully offline once the page is loaded

---

## 🖼️ Supported Image Types

| Type | Dimensions | Best for |
|------|-----------|----------|
| Primary / Poster | 680 × 1000 | Movie, show, collection covers |
| Backdrop | 1920 × 1080 | Background art behind metadata |
| Banner | 1000 × 185 | Wide horizontal title banners |
| Thumb | 1280 × 720 | Episode thumbnails |
| Logo | 800 × 310 | Transparent title logos |
| Clearart | 1000 × 562 | Transparent character/title art |
| Box | 750 × 1000 | Box-art style covers |
| Disc | 1000 × 1000 | Disc/bluray art |
| Custom | Any | Whatever you need |

---

## 🚀 How to Use

### 1. Choose your image type
Select from the **Image Type** dropdown. Canvas dimensions update automatically. Override width and height manually for custom sizes.

### 2. Set a background
- **Black** — clean black background
- **Transparent** — no background (best for Logo and Clearart)
- **Dark teal** — matches Jellyfin's UI palette
- **Custom color** — any color via picker
- **Background gradient** — 3-stop gradient with direction control
- **Pattern** — one of 6 built-in geometric patterns
- **Background image** — upload a photo or artwork (see [Background Image](#️-background-image) below)

### 3. Add your text
Type up to 4 lines of text. Each line is independent — leave a box empty to skip it. Text auto-scales to fill the canvas, or enter a fixed font size to lock it. Use the **Text Position** section to move the text block anywhere on the canvas using the 9-point anchor grid and X/Y offset sliders.

### 4. Pick a text style

| Style | Description |
|-------|-------------|
| **Gradient** | Multi-color gradient across the text — choose from presets or pick 3 custom colors with direction control |
| **Solid** | Flat single color |
| **Outline** | Hollow text with a colored stroke — adjustable fill, stroke color, and thickness |
| **Shadow** | Text with a soft drop shadow — adjustable shadow color and blur radius |
| **Neon** | Bright core with layered glow effect — best on dark backgrounds |
| **Stamp** | Bold fill with thick contrasting stroke, like a screen-print or rubber stamp |

### 5. Add a second text layer (optional)
Enable the **Second Text Layer** toggle to add an independent block of text — perfect for a subtitle, year, season label, or any supporting copy. Has its own font, size, alignment, color, opacity, and position relative to the main text (above, below, or pinned to top/bottom of canvas).

### 6. Add effects (optional)
- **Texture Overlay** — add grain, scanlines, halftone, or scratch textures on top of the background for a cinematic or retro feel
- **Pattern Background** — overlay a geometric pattern (dots, grid, diagonal, chevron, crosshatch, hexagons) with custom color and scale
- **Duotone** — remap your background image to two colors, mapping shadows to one and highlights to another
- **Shape Elements** — place a decorative line, circle, rectangle, diamond or triangle on the canvas with full style controls

### 7. Add a border (optional)
- **Width** — thickness in pixels
- **Color** — any color via the picker
- **Corner radius** — 0 for sharp corners, higher values for rounded
- **Style** — Solid, Gradient (matches your text gradient), or Inset Glow

### 8. Add a vignette (optional)
Enable the **Vignette** toggle to add a radial dark gradient from the edges inward. Adjustable intensity, spread, and color.

### 9. Add a logo or overlay image (optional)
Enable **Logo / Overlay Image** to upload a second image — a network logo, show logo, or any PNG. Position it using the 9-point grid, and control size (as % of canvas), opacity, and edge padding. Transparent PNGs work perfectly here.

### 10. Add a corner badge (optional)
Enable the **Corner Badge** to stamp a label on any corner. Choose from quick presets or type custom text. Configure corner, size, background color, and text color.

### 11. Export
- **Export PNG (with background)** — full image including all layers and background
- **Export PNG (transparent bg)** — removes the background, text and overlays only
- **Batch Export** — export multiple Jellyfin image types at once, each at the correct dimensions

Files are automatically named based on your text and image type, e.g. `thai-gl-series-primary.png`.

---

## 🖼️ Background Image

Upload any image (JPG, PNG, WebP, etc.) by clicking the drop zone or dragging a file onto it.

### Fit modes
| Mode | Description |
|------|-------------|
| Cover | Fills the canvas, cropping edges if needed |
| Contain | Fits the whole image inside the canvas |
| Stretch | Fills exactly, ignoring aspect ratio |
| Tile | Repeats the image as a pattern |
| Center | No scaling, centered as-is |

### Adjustments
- **Opacity** — 0% to 100%
- **Blur** — 0px to 40px Gaussian blur
- **Brightness** — 0% to 200%
- **Contrast** — 0% to 200%
- **Saturate** — 0% (greyscale) to 200% (vivid)
- **Blend mode** — Normal, Multiply, Screen, Overlay, Soft Light, Hard Light, Color Dodge, Color Burn, Luminosity

### Color overlay
Enable the color overlay toggle to add a flat color layer on top of the image before drawing text. Useful for darkening a busy photo so your text stays readable. Has its own color picker and opacity slider.

---

## 🎨 Creative Effects

### Texture Overlay
Add a film-like texture on top of your design. Four types available — **Grain** (random noise for a cinematic feel), **Scanlines** (horizontal bands for a retro CRT look), **Halftone** (dot grid for a print/comic style), **Scratches** (vertical light streaks for aged film). Each has its own intensity and blend mode control.

### Pattern Background
Six geometric patterns drawn directly on the canvas: **Dots**, **Grid**, **Diagonal**, **Chevron**, **Crosshatch**, **Hexagons**. Set any color, opacity, and scale. Patterns draw underneath the background image and text so everything still layers correctly.

### Duotone
Remaps every pixel of the canvas — shadow tones become Color 1, highlight tones become Color 2. Intensity slider blends between original and full duotone. Works on anything drawn before it — background photo, solid color, or gradient.

### Shape Elements
Add a single decorative shape to the canvas: **Horizontal line**, **Vertical line**, **Circle**, **Rectangle**, **Diamond**, or **Triangle**. Choose outline or filled style, set color, size, thickness, opacity and position (center, top, bottom, or behind the text).

---

## 💾 Presets

Save your current settings as a named preset and reload them with one click. Presets are stored in your browser's localStorage and persist between sessions.

### Export & Import
- **Export presets** — downloads a `.json` backup file of all your saved presets
- **Import presets** — loads presets from a previously exported file, merging with any you already have (duplicates skipped)

Use export/import to back up your presets, share them with others, or move them to a different browser or device.

---

## 🔤 Fonts

30 fonts organised into categories:

| Category | Fonts |
|----------|-------|
| Rounded & Friendly | Nunito, Righteous, Boogaloo |
| Bold & Display | Bebas Neue, Oswald, Anton, Russo One, Teko, Bangers, Abril Fatface, Alfa Slab One, Impact |
| Sci-Fi & Tech | Orbitron, Exo 2, Chakra Petch, Rajdhani, Kanit |
| Elegant & Serif | Cinzel, Playfair Display, Merriweather, Bree Serif, Georgia |
| Handwritten & Fun | Permanent Marker, Lobster, Creepster |
| Retro & Pixel | Press Start 2P, VT323, Courier New |
| System | Arial Rounded |

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Z` / `Cmd+Z` | Undo |
| `Ctrl+Y` / `Cmd+Shift+Z` | Redo |
| Scroll wheel on preview | Zoom in/out |
| Click + drag on preview | Pan when zoomed |
| Click zoom badge | Reset zoom to 100% |

---

## 💡 Tips

- **For Logo and Clearart types**, use transparent export with no background — these are designed to overlay on top of backdrops in Jellyfin
- **Neon style** works best with a pure black background and a vivid glow color
- **Gradient border** automatically matches your text gradient, keeping everything cohesive
- **Backdrop art** (1920×1080) works great with a background photo + dark color overlay + shadow or solid text
- **Second text layer** is perfect for adding a year or episode count in a smaller, lighter font below your main title
- **Logo overlay** with a transparent PNG in the bottom corner is a clean way to brand collection art consistently
- **Corner badges** like 4K or DUBBED are useful for collection posters where you want the format visible at a glance
- **Duotone + vignette** is a great combination for a dramatic, cinematic poster look from any photo
- **Grain texture** with Overlay blend mode adds subtle depth to flat gradient backgrounds
- **Batch export** saves a lot of time when creating art for an entire collection — design once, export all sizes at once
- **Export your presets** as a JSON file regularly — this is your only backup if you switch browsers or clear your cache
- The **font size field** accepts any value — useful when you want consistent sizing across multiple exports for the same collection

---

## 🛠️ Tech Stack

Pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build step. Everything runs in a single self-contained `.html` file directly in the browser using the Canvas API.

---

## 🤝 Contributing

Contributions, suggestions, and bug reports are welcome. Open an issue or submit a pull request.

---

## 📄 License

MIT License — free to use, modify, and distribute.
