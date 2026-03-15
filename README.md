# 🎨 Jellyfin Artwork Generator

A free, browser-based tool for creating custom artwork for your [Jellyfin](https://jellyfin.org) media server — posters, backdrops, banners, logos, and more. No sign-up, no install, no watermarks. Everything runs locally in your browser.

**[→ Open the Generator](https://loyalwolf.github.io/Jellyfin-Artwork-Generator)**

---

## ✨ Features

- **All Jellyfin image types** — Primary, Backdrop, Banner, Thumb, Logo, Clearart, Box, Disc, and custom dimensions
- **Live preview** — changes render instantly as you type or adjust settings
- **Background image support** — upload any image with full control over opacity, blur, brightness, contrast, saturation, blend mode, and color overlay
- **6 text styles** — Gradient, Solid, Outline, Shadow, Neon, Stamp
- **Gradient presets** — 8 curated presets with full custom color control (3-stop gradients, 4 directions)
- **Border options** — color, width, corner radius, and style (solid, gradient-matched, inset glow)
- **PNG export** — export at full resolution with or without background (transparent export ideal for Logo and Clearart types)
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
Select from the **Image Type** dropdown. The canvas dimensions update automatically. You can also override the width and height manually for custom sizes.

### 2. Set a background
Choose from:
- **Black** — clean black background
- **Transparent** — no background (best for Logo and Clearart)
- **Dark teal** — matches Jellyfin's UI palette
- **Custom color** — pick any color
- **Image** — upload a photo or artwork (see [Background Image](#background-image) below)

### 3. Add your text
Type up to 4 lines of text. Each line is independent — leave a box empty to skip it. Text auto-scales to fill the canvas, or enter a fixed font size to lock it.

### 4. Pick a text style
| Style | Description |
|-------|-------------|
| **Gradient** | Multi-color gradient across the text. Choose from presets or pick 3 custom colors with direction control |
| **Solid** | Flat single color |
| **Outline** | Hollow text with a colored stroke. Adjustable fill, stroke color, and thickness |
| **Shadow** | Text with a soft drop shadow. Adjustable shadow color and blur radius |
| **Neon** | Bright core with layered glow effect — best on dark backgrounds |
| **Stamp** | Bold fill with thick contrasting stroke, like a screen-print or rubber stamp |

### 5. Add a border (optional)
Enable the border toggle and configure:
- **Width** — thickness in pixels
- **Color** — any color via the picker
- **Corner radius** — 0 for sharp corners, higher values for rounded
- **Style** — Solid, Gradient (matches your text gradient), or Inset Glow

### 6. Export
- **Export PNG (with background)** — full image including background color/image
- **Export PNG (transparent bg)** — text and border only, no background

Files are automatically named based on your text and image type, e.g. `series-primary.png`.

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
Enable the color overlay toggle to add a flat color on top of the image before drawing text. Useful for darkening a busy photo so your text stays readable. Has its own color picker and opacity slider.

---

## 💡 Tips

- **For Logo and Clearart types**, use transparent export and a transparent or no background — these image types are designed to overlay on top of backdrops in Jellyfin
- **Neon style** works best with a pure black background and a dark-colored glow
- **Gradient border style** automatically matches whatever gradient you've set for your text, keeping everything cohesive
- **Backdrop images** (1920×1080) work well with a background photo + dark overlay + solid or shadow text
- The **font size field** accepts any value — useful when you want consistent sizing across multiple exports

---

## 🛠️ Tech Stack

Pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build step. Everything runs in a single self-contained `.html` file directly in the browser using the Canvas API.

---

## 🤝 Contributing

Contributions, suggestions, and bug reports are welcome. Open an issue.

---

## 📄 License

MIT License — free to use, modify, and distribute.
