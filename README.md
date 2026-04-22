# GifCam

<p align="center">
  <b>Screen capture for Windows — Screenshot · GIF · MP4 · Pro video editor</b>
  <img width="387" height="358" alt="image" src="https://github.com/user-attachments/assets/94571d45-10a1-43e6-8c39-e5d717ad05a1" />

<img width="545" height="307" alt="image" src="https://github.com/user-attachments/assets/cb6377df-8cc7-4070-9e5b-355c05ff0e64" />

</p>

<p align="center">
  <a href="https://github.com/kuoungseok/gifcam/releases/latest">
    <b>▶ Download the latest installer</b>
  </a>
</p>

---

## What makes GifCam different

### ⚡ Fast-motion and slow-motion in the **same** video
Select any range on the track and dial it from **0.25× up to 16× speed**.
Keep the rest at normal 1× — or layer multiple speed segments on top of
each other. A tutorial can zip through setup at 4× then settle into 1× for
the key steps, all in one clip.

### 🎞 Layered multi-track playback
Stack multiple clips. The top track plays by default; cut regions fall
through to the track beneath, and short tracks reveal the one under them
once they end. No timeline gaps.

### ⚙ Windows Graphics Capture backend
GPU-accelerated capture via the modern WGC API — 60 fps on large regions
without the black-frame and DPI quirks of GDI / BitBlt, even on mixed-DPI
multi-monitor setups.

### 📋 Subtitles with or without a box
Per-subtitle toggle. Show the classic semi-transparent box, or go box-free
with an outline + drop shadow. Burned into the exported MP4.

### 🖱 One-click "Quick paste"
Record, then press the **Quick paste** button — GifCam copies the file to
the clipboard, refocuses the window you were editing (Confluence, Jira,
Slack, Notion, KakaoTalk, Discord...), and sends `Ctrl+V` for you.

---

## Features at a glance

- **Screenshot / GIF / Video** modes with a Win11-Snipping-Tool–style UI
- **Multi-monitor, mixed-DPI aware** region selector
- **GIF encoder** with per-frame adaptive palette (+ automatic `gifski` /
  `gifsicle` if installed)
- **MP4 (H.264)** export with per-segment speed, cuts, and subtitle burn-in
- **Multi-language UI** — 한국어 · English · 日本語 · Deutsch
  (auto-detected from Windows locale, live switchable)
- **Keyboard shortcuts** — `Ctrl+Shift+N` new capture, `Ctrl+1/2/3` mode
  switch, `Ctrl+O` save folder, `Ctrl+,` settings
- **Portable or installed** — either run `GifCam.exe` directly or use the
  installer which registers in *Settings → Apps* for normal Windows
  uninstall

## Install

### Installer (recommended)

1. Download **`GifCam-Setup-1.0.0.exe`** from the
   [**Releases** page](https://github.com/kuoungseok/gifcam/releases/latest)
2. Double-click and follow the wizard — no admin rights required
3. Installed to `%LOCALAPPDATA%\GifCam`, listed in *Settings → Apps*

### Portable

Download **`GifCam-1.0.0-portable.zip`**, unzip anywhere, run
`GifCam.exe`. Delete the folder to remove. Captured files live in
`~/Videos/GifCam` regardless of install method.

## System requirements

- Windows 10 1903+ or Windows 11
- x64

## Support the project

If GifCam saves you time, consider sending a few dollars:

- **PayPal** — https://paypal.me/KyoungseokKo
- **GitHub Sponsors** — https://github.com/sponsors/kuoungseok
- **Star this repo ⭐** — biggest motivation, costs nothing

## Author

**KyoungSeok Ko** ([artmouse](https://github.com/kuoungseok))

## License

[MIT](LICENSE)
