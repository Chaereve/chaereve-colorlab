# 🎨 ACO Color Viewer Pro

> **🇬🇧 English** · [🇻🇳 Tiếng Việt](README.vi.md)

A tool to **view, mix, and export Photoshop (`.aco`) color palettes** — running entirely **in your browser**. No installation, no sign-up, no data upload.

> Everything is processed **100% locally** on your device.

**🌐 Bilingual UI:** the app has a built-in **Vietnamese ↔ English** language switcher (the `EN` / `VI` button in the top-right corner).

---

## ✨ Features

### 📁 View ACO
- Drag & drop (or click) a `.aco` file to open it.
- Supports **ACO v1 & v2**, reads **color names** and the RGB / HSB / CMYK / Lab / Grayscale color spaces.
- Each color shows an **index number**, name, HEX, RGB and its original color space.
- **Search** by name/HEX/RGB and **sort** by hue, lightness, saturation, or name.

### 📋 Copy
- Click a swatch to copy its code (**HEX / RGB / HSL** — selectable).
- **Copy all** as: HEX list, CSS variables, SCSS, JSON, or RGB list.

### 🎨 Mix colors (standalone — no ACO required)
- Add colors with the **color picker** or **open an ACO file** right in this tab.
- A selection grid lets you **exclude colors you don't want to mix** with one click.
- **Re-adjust your selection** without re-uploading the file.
- Ratios **auto-equalize** by color count; drag a slider to tweak each one.
- **Mix history** is saved automatically; click to copy again.

### 🎲 Random colors (per member)
- Generate 1–100 random colors for each "member", either fully random or within a chosen color family (red / orange / yellow / green / cyan / blue / purple / pink), with optional no-duplicate mode.

### 🛠 Design tools
- **Palette Generator** — complementary / analogous / triadic / split / tetradic.
- **Gradient Generator** — linear/radial CSS gradient with copy-to-clipboard.
- **Contrast Checker** — WCAG ratio with AA/AAA badges.
- **Color Blindness Preview** — protanopia / deuteranopia / tritanopia / grayscale.
- **Image → Palette / Eyedropper** — click an image to pick a color, or extract dominant colors.
- **Color detail panel** — HEX / RGB / HSL / HSV / CMYK / Lab, luminance, contrast.
- **Duplicate detector** and **similar-color finder**.

### ⬇ Export
- **PNG / SVG / CSS / JSON / TXT** with layout, size, label and background options (including transparent).
- **ACO export** (v2, with color names) of your selected colors.

### 🌙 UI
- **Dark / light** theme (dark is the default).
- **Language switcher: Vietnamese / English**.
- Smooth animations and a mobile-first layout (bottom nav, bottom sheets, large touch targets).

### 📲 Install as an app (PWA)
- Installable on **desktop (Windows/macOS/Linux)** and **mobile (Android/iOS)**.
- Has its own icon, opens in a standalone window, and works **offline**.

### 🖥 Desktop version (.exe)
- Packaged as a **Windows installer** using Electron — see the `electron-app/` folder.

---

## 🚀 Usage

### On desktop / mobile
Just open `index.html` in any browser (double-click it), or visit the deployed URL.

### Quick flow
1. Open the **📁 View ACO** tab → drag & drop a `.aco` file.
2. Click a color to copy it, or tick several colors to export them.
3. Open the **🎨 Mix colors** tab → add colors → see the mix result instantly.
4. Click **⬇ Export image & data** to download the palette.

---

## 🌐 Language switcher

Click the **`EN` / `VI`** button (next to the theme button, top-right) to switch the whole interface between **English** and **Vietnamese**. Your choice is remembered across sessions.

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

## 🖥 Run locally (no deploy needed)

```bash
# Option 1: double-click index.html
# Option 2: local server (optional)
python3 -m http.server 8080
# then open http://localhost:8080 in your browser
```

---

## 🌍 Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `aco-color-viewer`).
2. Upload the contents of the `aco-color-viewer/` folder (including the `icons/` folder).
3. Go to **Settings → Pages → Source** → **Deploy from a branch** → branch `main`, folder `/ (root)` → **Save**.
4. Wait 1–2 minutes, then visit: `https://<your-username>.github.io/aco-color-viewer/`

> The app is a **single self-contained HTML file** (no backend, no CDN), so it runs on any static host: GitHub Pages, Netlify, Vercel, Cloudflare Pages…

---

## 🌐 Making your GitHub page bilingual (2 languages)

You already have a **language switcher inside the app** (EN/VI button). For the **repository page / README** itself, GitHub does not auto-translate READMEs, so use one of these approaches:

### Method A — Two README files with a language switcher (recommended)
1. Keep `README.md` in **English** (default shown).
2. Create `README.vi.md` in **Vietnamese**.
3. At the top of **both** files, add a small language switcher:

   ```markdown
   [🇬🇧 English](README.md) · [🇻🇳 Tiếng Việt](README.vi.md)
   ```

Visitors land on the English README and switch languages with one click.

### Method B — Single file with two stacked sections
1. Put everything in one `README.md`.
2. Use a table of contents with anchors:

   ```markdown
   [English](#english) · [Tiếng Việt](#tiếng-việt)

   ## English
   ...english content...

   ## Tiếng Việt
   ...Vietnamese content...
   ```

### Method C — Full bilingual website (Jekyll)
GitHub Pages supports Jekyll, which can serve a multilingual static site. This is heavier and only needed if you want more than a README.

> In all cases, the **app itself** is already bilingual via the EN/VI button, so end users always get the right language regardless of the README.

---

## 🔄 Updating GitHub and rebuilding the .exe

After you change something (e.g. `index.html`), you need to update both the web version and the desktop `.exe`. Full step-by-step instructions are in **[HUONG_DAN_TUNG_BUOC.md](HUONG_DAN_TUNG_BUOC.md)** (Vietnamese). Quick summary:

### Update the web version (GitHub)
1. Open your repository on GitHub.
2. Go to the file you changed → **Edit (pencil)** → paste the new content → **Commit changes**. Or use **Add file → Upload files** to replace a whole file/folder.
3. GitHub Pages rebuilds automatically — refresh the live URL after 1–2 minutes (hard refresh with **Ctrl+F5**).

### Update the .exe (Windows)
1. Copy the updated `index.html` into `electron-app/` on your Windows machine (overwrite the old one).
2. Open a command prompt in `electron-app/` and run:
   ```bash
   npm run dist:win
   ```
   (run `npm install` first if it's a fresh copy)
3. The new `.exe` appears in `electron-app/dist/`. Replace the old installer/portable exe with the new one.

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

- **English user guide:** [USER_GUIDE.md](USER_GUIDE.md)
- **Vietnamese user guide:** [HUONG_DAN_SU_DUNG.md](HUONG_DAN_SU_DUNG.md)
- **Step-by-step (deploy + .exe build, Vietnamese):** [HUONG_DAN_TUNG_BUOC.md](HUONG_DAN_TUNG_BUOC.md)

---

## 🛠 Tech stack

- Pure **HTML + CSS + JavaScript** (Vanilla JS) — no framework, no external libraries.
- Binary ACO parsing with `DataView`; drawing/export with the Canvas API.
- Fully client-side.

---

## 📄 License

Free to use for personal and commercial work.
