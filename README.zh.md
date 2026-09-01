# 🎨 Chaereve ColorLab

<p align="center">
  <a href="https://github.com/chaereve/chaereve-colorlab/releases"><img alt="下载" src="https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD-2ea043?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-22d3ee?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-1a3fd6?style=for-the-badge"></a>
</p>

一款用于**查看、混合和导出 Photoshop（`.aco`）调色板**的工具——完全在**浏览器中**运行。无需安装、无需注册、无需上传数据。

> 所有数据都在您的设备上**100% 本地**处理。

**🌐 多语言界面（6 种语言）：** 越南语、英语、中文（简体）、한국어、日本語、Español——在**⚙️ 设置**中切换。

---

## ✨ 功能

### 📁 查看 ACO
- 拖放（或点击）`.aco` 文件即可打开。
- 支持 **ACO v1 与 v2**，可读取**颜色名称**以及 RGB / HSB / CMYK / Lab / 灰度色彩空间。
- 每个颜色显示**序号**、名称、HEX、RGB 及其原始色彩空间。
- 按名称/HEX/RGB **搜索**，按色相、明度、饱和度或名称**排序**。
- **高级搜索**——按范围筛选 `hue:0-60`、`sat:>50`、`light:40-80`，或用 `similar:#FF0000` 查找相近颜色。

### ✏️ 编辑调色板（就地编辑）
- **重命名**颜色（✏️）、**删除**（🗑）或**添加**新颜色——然后**保存回 .aco**。
- 完整的**撤销 / 重做**（最多 60 步）。
- **右键**色块可打开快捷菜单（复制 / 详情 / 重命名 / 导出 / 删除）。

### 📋 复制
- 点击色块复制其代码（**HEX / RGB / HSL**——可选）。
- **全部复制**为：HEX 列表、CSS 变量、SCSS、JSON、RGB、**Tailwind 配置**或 **Styled Components**。

### 🎨 混合颜色（独立使用——无需打开 ACO）
- 用**取色器**添加颜色，或直接在本标签页**打开 ACO 文件**。
- 选择网格可一键**排除不想混合的颜色**。
- 无需重新上传即可**重新调整选择**。
- 比例按颜色数量**自动均分**；拖动滑块逐个调整。
- **混合历史**自动保存，点击即可再次复制。

### 🎲 随机颜色（按成员）
- 为每个“成员”生成 1–100 个随机颜色，可完全随机，也可限定色系（红 / 橙 / 黄 / 绿 / 青 / 蓝 / 紫 / 粉），并可选不重复模式。

### 🛠 设计工具
分为两个标签页——**🧩 生成**与 **🔍 分析**：
- **调色板生成器**——互补 / 近似 / 三角 / 分裂 / 四角。
- **渐变生成器**——线性 / 径向 / **圆锥** CSS 渐变，一键复制。
- **图片 → 调色板 / 取色器**——点击图片取色，提取主色，并**直接导出为 .aco**。
- **预设与模板**——内置 Material Design、Tailwind、品牌色、粉彩和大地色系调色板。
- **对比度检查器**——WCAG 对比度及 AA/AAA 徽章。
- **无障碍审计**——调色板对白/黑文字达到 AA 的比例。
- **调色板统计**——平均饱和度/明度及色相分布图。
- **色盲预览**——红色盲 / 绿色盲 / 蓝色盲 / 灰度。
- **颜色详情面板**——HEX / RGB / HSL / HSV / CMYK / Lab、亮度、对比度。
- **重复检测器**和**相近颜色查找器**。

### 📦 批量处理
- 一次性打开**多个 .aco 文件**，然后**合并**为一个调色板（可选去重）或**导出合并后的 .aco**。

### 🔗 分享调色板
- 生成**分享链接**（`?palette=...`），对当前调色板进行编码——任何人打开链接都能看到相同的颜色，无需服务器。

### 📐 渐变 (.grd)
- 打开 Photoshop **渐变文件**（`.grd`，**v3 与 v5**）——纯色与噪点渐变。
- **预览**每个渐变，然后**编辑**色标、透明度标、中点、平滑度以及噪点参数（种子、粗糙度、最小/最大）。
- **添加 / 删除渐变**和色标，然后**保存回 `.grd`**。
- 将渐变导出为 **CSS `linear-gradient`** 或 **SVG**，并将其颜色**提取到 `.aco`** 或直接送入查看器。

### ⬇ 导出
- **PNG / SVG / CSS / JSON / TXT**，含布局、尺寸、标签和背景选项（包括透明）。
- 将所选颜色**导出为 .aco**（v2，含颜色名称）。

### 🌙 界面——玻璃拟态
- **玻璃拟态**设计：磨砂玻璃面板、柔和模糊与氛围光——精致如 macOS/iOS。
- **深色 / 浅色 / 自动**主题（默认跟随系统）。
- **6 种语言**：越南语、英语、中文（简体）、한국어、日本語、Español——可在**⚙️ 设置**中切换。
- 流畅的动画和移动优先的布局（底部导航、底部面板、大触控目标）。

### ⚙️ 设置
- **外观**——浅色、深色或自动主题。
- **强调色**——重绘整个界面（logo、标签页、按钮、发光效果）。
- **语言**与**字号**（小 / 中 / 大）。
- **音效**——点击、复制和通知时播放轻柔音效（开/关）。
- **动画效果**开/关、**清除已保存数据**，以及**关于**说明。

### 📲 安装为应用（PWA）
- 可安装到**桌面（Windows/macOS/Linux）**和**移动端（Android/iOS）**。
- 拥有独立图标、独立窗口打开，并可**离线**工作。

### 🖥 桌面版（Windows）
- 使用 Electron 打包为**原生 Windows 桌面应用**——见 `electron-app/` 文件夹。
- 构建 **Windows** 安装包：`.exe`（安装程序 + 便携版）。
- 应用 logo 为**圆角方形**，如同现代应用。

---

## 🚀 使用

### 桌面 / 移动端
在任何浏览器中打开 `index.html`（双击即可），或访问已部署的网址。

### 快速流程
1. 打开 **📁 查看 ACO** 标签页 → 拖放 `.aco` 文件。
2. 点击颜色复制，或勾选多个颜色导出。
3. 打开 **🎨 混合颜色** 标签页 → 添加颜色 → 立即查看混合结果。
4. 点击 **⬇ 导出图片与数据** 下载调色板。
5. 打开 **📐 渐变** 标签页 → 放入 `.grd` 文件以查看和编辑 Photoshop 渐变。
6. 打开 **⚙️ 设置** 切换主题、强调色、语言和字号。

---

## 🌐 语言（6 种）

打开 **⚙️ 设置**（右上角齿轮按钮），在**语言**菜单中选择：越南语、英语、中文（简体）、한국어、日本語、Español。整个界面即时切换，选择会被记住。

**本仓库的 README 与使用指南均有 6 种语言：**

| 语言 | README | 使用指南 |
|------|--------|----------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |
| 🇨🇳 中文 (简体) | [README.zh.md](README.zh.md) | [USER_GUIDE.zh.md](USER_GUIDE.zh.md) |
| 🇰🇷 한국어 | [README.ko.md](README.ko.md) | [USER_GUIDE.ko.md](USER_GUIDE.ko.md) |
| 🇯🇵 日本語 | [README.ja.md](README.ja.md) | [USER_GUIDE.ja.md](USER_GUIDE.ja.md) |
| 🇪🇸 Español | [README.es.md](README.es.md) | [USER_GUIDE.es.md](USER_GUIDE.es.md) |

---

## 📲 安装为应用（PWA）

应用部署（通过 HTTPS）后，即可将其安装为真正的应用：

| 平台 | 方法 |
|------|------|
| **桌面**（Chrome/Edge） | 打开网址 → 点击 **📲** 按钮或地址栏的安装图标 → **安装** |
| **Android**（Chrome） | 打开网址 → **⋮** 菜单 → **添加到主屏幕** |
| **iPhone/iPad**（Safari） | 打开网址 → **分享**按钮 → **添加到主屏幕** |

> **重要：** PWA 必须通过 **HTTPS** 提供服务（GitHub Pages、Netlify、Vercel 均可）。直接打开 `file://` 无法安装。

---

## ❓ 常见问题

**我的数据会被上传到哪里吗？**
不会。一切都在浏览器中运行——不会通过网络发送任何内容。

**文件打开了但没有颜色？**
检查是否为有效的 `.aco` 文件。部分软件导出的 ACO 结构不规范。

**颜色混合是如何工作的？**
应用按比例混合颜色（加权平均）——像调颜料一样。拖动滑块让某个颜色“更重”。

**如何只混合文件中的部分颜色？**
在 **混合颜色** 标签页打开 ACO → 点击取消不想混合的颜色 → 点击**添加颜色到混合**。

---

## 📚 指南

使用指南（6 种语言）：
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md) · 🇨🇳 [USER_GUIDE.zh.md](USER_GUIDE.zh.md) · 🇰🇷 [USER_GUIDE.ko.md](USER_GUIDE.ko.md) · 🇯🇵 [USER_GUIDE.ja.md](USER_GUIDE.ja.md) · 🇪🇸 [USER_GUIDE.es.md](USER_GUIDE.es.md)

---

## 📄 许可证

可自由用于个人与商业用途。
