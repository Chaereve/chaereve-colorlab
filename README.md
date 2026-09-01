# 🎨 Chaereve ColorLab

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-22d3ee?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-1a3fd6?style=for-the-badge"></a>
</p>

A tool to **view, mix, and export Photoshop (`.aco`) color palettes** — running entirely **in your browser**. No installation, no sign-up, no data upload.

> Everything is processed **100% locally** on your device.

**🌐 Multilingual UI (6 languages):** Vietnamese, English, 中文 (简体), 한국어, 日本語, Español — switch in **⚙️ Settings**.

---

## ✨ Features

### 📁 View ACO
- Drag & drop (or click) a `.aco` file to open it.
- Supports **ACO v1 & v2**, reads **color names** and the RGB / HSB / CMYK / Lab / Grayscale color spaces.
- Each color shows an **index number**, name, HEX, RGB and its original color space.
- **Search** by name/HEX/RGB and **sort** by hue, lightness, saturation, or name.
- **Advanced search** — filter by ranges with `hue:0-60`, `sat:>50`, `light:40-80`, or find near-colors with `similar:#FF0000`.

### ✏️ Edit palette (in-place)
- **Rename** colors inline (✏️), **delete** (🗑), or **add** new colors — then **save back to .aco**.
- Full **undo / redo** (up to 60 steps).
- **Right-click** any swatch for a quick menu (copy / details / rename / export / delete).

### 📋 Copy
- Click a swatch to copy its code (**HEX / RGB / HSL** — selectable).
- **Copy all** as: HEX list, CSS variables, SCSS, JSON, RGB, **Tailwind config**, or **Styled Components**.

### 🎨 Mix colors (standalone — no ACO required)
- Add colors with the **color picker** or **open an ACO file** right in this tab.
- A selection grid lets you **exclude colors you don't want to mix** with one click.
- **Re-adjust your selection** without re-uploading the file.
- Ratios **auto-equalize** by color count; drag a slider to tweak each one.
- **Mix history** is saved automatically; click to copy again.

### 🎲 Random colors (per member)
- Generate 1–100 random colors for each "member", either fully random or within a chosen color family (red / orange / yellow / green / cyan / blue / purple / pink), with optional no-duplicate mode.

### 🛠 Design tools
Split into two tabs — **🧩 Create** and **🔍 Analyze**:
- **Palette Generator** — complementary / analogous / triadic / split / tetradic.
- **Gradient Generator** — linear / radial / **conic** CSS gradient with copy-to-clipboard.
- **Image → Palette / Eyedropper** — click an image to pick a color, extract dominant colors, and **export them straight to .aco**.
- **Presets & Templates** — built-in Material Design, Tailwind, Brand Colors, Pastel and Earth Tones palettes.
- **Contrast Checker** — WCAG ratio with AA/AAA badges.
- **Accessibility Audit** — % of the palette passing AA against white/black text.
- **Palette Statistics** — average saturation/lightness and a hue-distribution chart.
- **Color Blindness Preview** — protanopia / deuteranopia / tritanopia / grayscale.
- **Color detail panel** — HEX / RGB / HSL / HSV / CMYK / Lab, luminance, contrast.
- **Duplicate detector** and **similar-color finder**.

### 📦 Batch processing
- Open **multiple .aco files** at once, then **merge** them into one palette (with optional dedup) or **export a merged .aco**.

### 🔗 Share palette
- Generate a **shareable link** (`?palette=...`) that encodes the current palette — anyone opening the link sees the same colors, no server needed.

### 📐 Gradient (.grd)
- Open Photoshop **gradient files** (`.grd`, **v3 & v5**) — solid and noise gradients.
- **Preview** each gradient, then **edit** color stops, transparency stops, midpoint, smoothness, and noise parameters (seed, roughness, min/max).
- **Add / remove gradients** and stops, then **save back to `.grd`**.
- Export a gradient as **CSS `linear-gradient`** or **SVG**, and **extract its colors to `.aco`** or straight into the Viewer.

### ⬇ Export
- **PNG / SVG / CSS / JSON / TXT** with layout, size, label and background options (including transparent).
- **ACO export** (v2, with color names) of your selected colors.

### 🌙 UI — glassmorphism
- **Glassmorphism** design: frosted-glass panels, soft blur and ambient light — polished like macOS/iOS.
- **Dark / light / auto** theme (follows your system by default).
- **6 languages**: Vietnamese, English, 中文 (简体), 한국어, 日本語, Español — switchable in **⚙️ Settings**.
- Smooth animations and a mobile-first layout (bottom nav, bottom sheets, large touch targets).

### ⚙️ Settings
- **Appearance** — light, dark or auto theme.
- **Accent color** — recolor the whole UI (logo, tabs, buttons, glow).
- **Language** and **font size** (small / medium / large).
- **Sound effects** — subtle sounds for clicks, copies and notifications (on/off).
- **Motion effects** on/off, **clear saved data**, and an **About** box.

### 📲 Install as an app (PWA)
- Installable on **desktop (Windows/macOS/Linux)** and **mobile (Android/iOS)**.
- Has its own icon, opens in a standalone window, and works **offline**.

### 🖥 Desktop version (Windows / macOS / Linux)
- Packaged as a **native desktop app** using Electron — see the `electron-app/` folder.
- Build installers for every OS: **Windows** (`.exe` installer + portable), **macOS** (`.dmg`) and **Linux** (`.AppImage`).
- The app logo is **round**, like modern apps.

---

## 🚀 Usage

### On desktop / mobile
Just open `index.html` in any browser (double-click it), or visit the deployed URL.

### Quick flow
1. Open the **📁 View ACO** tab → drag & drop a `.aco` file.
2. Click a color to copy it, or tick several colors to export them.
3. Open the **🎨 Mix colors** tab → add colors → see the mix result instantly.
4. Click **⬇ Export image & data** to download the palette.
5. Open the **📐 Gradient** tab → drop a `.grd` file to view and edit Photoshop gradients.
6. Open the **⚙️ Settings** tab to switch theme, accent color, language and font size.

---

## 🌐 Languages (6)

Open **⚙️ Settings** (the gear button, top-right) and pick a language from the **Language** menu: Vietnamese, English, 中文 (简体), 한국어, 日本語, Español. The whole interface switches instantly and your choice is remembered across sessions.

This repository's **README and User Guide are available in all 6 languages**:

| Language | README | User Guide |
|----------|--------|------------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |
| 🇨🇳 中文 (简体) | [README.zh.md](README.zh.md) | [USER_GUIDE.zh.md](USER_GUIDE.zh.md) |
| 🇰🇷 한국어 | [README.ko.md](README.ko.md) | [USER_GUIDE.ko.md](USER_GUIDE.ko.md) |
| 🇯🇵 日本語 | [README.ja.md](README.ja.md) | [USER_GUIDE.ja.md](USER_GUIDE.ja.md) |
| 🇪🇸 Español | [README.es.md](README.es.md) | [USER_GUIDE.es.md](USER_GUIDE.es.md) |

---

## 📲 Install as an app (PWA)

Once the app is deployed (over HTTPS), you can install it as a real app:

| Platform | How |
|----------|-----|
| **Desktop** (Chrome/Edge) | Open the URL → click the **📲** button (top-right) or the install icon in the address bar → **Install** |
| **Android** (Chrome) | Open the URL → **⋮** menu → **Add to Home Screen** |
| **iPhone/iPad** (Safari) | Open the URL → **Share** button → **Add to Home Screen** |

> **Important:** PWAs must be served over **HTTPS** (GitHub Pages, Netlify and Vercel all do this). You cannot install when opening a `file://` directly.

---

## 🌐 Language-switch buttons

Every `README.<lang>.md` starts with a **language-switch button bar** (the buttons at the top). To add it to a new README, paste this at the very top:

```markdown
<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-1a3fd6?style=for-the-badge"></a>
</p>
```

Use a different color (e.g. `22d3ee`) for the **current** language's button.

---

## ❓ FAQ

**Is my data uploaded anywhere?**
No. Everything runs in your browser — nothing is sent over the network.

**The file opens but no colors appear?**
Check that it's a valid `.aco` file. Some apps export ACO with a non-standard structure.

**How does color mixing work?**
The app blends colors by ratio (weighted average) — like mixing paint. Drag a slider to make a color "heavier".

**How do I mix only some colors from a file?**
Open the ACO in the **Mix colors** tab → click to deselect the colors you don't want → click **Add colors to mix**.

---

## 📚 Guides

User guide (all 6 languages):
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md) · 🇨🇳 [USER_GUIDE.zh.md](USER_GUIDE.zh.md) · 🇰🇷 [USER_GUIDE.ko.md](USER_GUIDE.ko.md) · 🇯🇵 [USER_GUIDE.ja.md](USER_GUIDE.ja.md) · 🇪🇸 [USER_GUIDE.es.md](USER_GUIDE.es.md)

Deploy & build (step-by-step): [HUONG_DAN_TUNG_BUOC.md](HUONG_DAN_TUNG_BUOC.md)

---

## 📄 License

Free to use for personal and commercial work.
