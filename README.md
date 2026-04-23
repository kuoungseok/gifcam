# GifCam

**A Windows screen recorder for people who edit what they record.**
Scribble and bubble freely on the video. Speed up the boring parts, slow down the important ones. Drop fades between cuts. Paste it straight into Jira or Confluence.

[**▶ Download the latest installer**](https://github.com/kuoungseok/gifcam/releases/latest)

---

## Why I built this

I write a lot of work reports — bug reports, PR demos, internal docs — and I put GIFs in all of them. I wanted one tool that let me record a region, speed up the setup, slow down the key steps, scribble annotations, and paste the result straight into Jira. No cloud upload, no subscription, no forty-tab menu.

So I built GifCam for myself. It turned out my coworkers wanted it too. Now it's on GitHub. Free, open source, no ads, no account.

**— KyoungSeok Ko**

---

## What makes GifCam different

### 🖌 Scribble and bubble on the video

Click anywhere on the preview and a paint dialog opens over the current frame. Pen, eraser, 8 preset colors + custom picker, width & opacity — plus **speech bubbles** with inline text editing and a toggleable left/right tail. Strokes and bubbles **render during playback** and are **burned into the exported MP4** at the exact time they appeared.

I couldn't find another free Windows tool that does this the way I wanted, so I built it.

![Paint dialog](docs/screenshots/paint-dialog.png)

### ⚡ Fast-forward and slow-motion in the **same** video

Select any range on the timeline and dial it from **0.25× up to 16× speed**. A tutorial can zip through setup at 4× then settle into 1× for the key steps, all in one clip.

![Pro video editor](docs/screenshots/video-editor.png)

### 🎬 Drag-drop fade transitions

Grab the **Fade** card and drop it on the track — the width of the placed actor is its duration. Drag the edges to resize. Right-click to toggle **Fade In / Fade Out / In + Out**. Preview shows the effect live.

### 🖱 One-click paste to Jira / Confluence / Slack

Record, then press **Quick paste**. GifCam copies the file to the clipboard, refocuses the window you were editing, and sends `Ctrl+V` for you. No upload. No cloud. Just a file.

### ⚙ Modern Windows Graphics Capture backend

GPU-accelerated capture via the WGC API — 60 fps on large regions without the black-frame and DPI quirks of the old GDI/BitBlt approach. Works correctly on mixed-DPI multi-monitor setups (sub-monitor capture fixed in 1.3).

---

## At a glance

| | GifCam 1.3 |
|---|---|
| **Price** | Free, MIT license |
| **Modes** | Screenshot / GIF / MP4 video |
| **Theme** | Full dark mode (5-level palette) |
| **Editor** | Multi-track timeline, per-segment speed, paint, speech bubbles, fades, subtitles |
| **Export** | GIF (adaptive palette, optional gifski/gifsicle), MP4 (H.264) |
| **Zoom** | Mouse-wheel on timelines (video + GIF) |
| **Languages** | 한국어 · English · 日本語 · Deutsch |
| **Cloud upload** | None — everything stays on your machine |
| **Shortcuts** | `Ctrl+Shift+N` new capture, `Ctrl+1/2/3` mode switch |

---

## Screenshots

### Main window

![GifCam main window](docs/screenshots/main-window.png)

Windows 11 Snipping Tool–style interface in a full dark theme. Pick a mode, hit **New capture**, drag to select. The violet **Open pro video editor** button is a one-click entry to the multi-track editor.

### Subtitles

![Subtitle editor](docs/screenshots/subtitle-editor.png)

Time-aligned captions with an optional background box. Burned into the exported MP4.

---

## Install

1. Download **`GifCam-Setup-1.3.0.exe`** from the [**Releases** page](https://github.com/kuoungseok/gifcam/releases/latest)
2. Double-click and follow the wizard — no admin rights required
3. Installed to `%LOCALAPPDATA%\GifCam`, listed in *Settings → Apps*

Captured files live in `~/Videos/GifCam` by default.

**System requirements:** Windows 10 1903+ or Windows 11, x64.

---

## Support the project

I maintain GifCam in my spare time. If it saves you time at work, a coffee's worth keeps me shipping updates.

- ☕ **PayPal** — <https://paypal.me/KyoungseokKo>
- 🏦 **Toss Bank** (KRW) — `1001-5567-2524` 고경석

Not asking for a paycheck — just a signal that this is worth maintaining.

---

## Changelog highlights

- **1.3** — Full dark theme; speech bubbles; drag-drop fade transitions; mouse-wheel timeline zoom; sub-monitor capture fix; safer overwrite export
- **1.2** — Paint-on-preview with live playback rendering
- **1.1** — Multi-track timeline, per-region speed (0.25×–16×)
- **1.0** — Initial release: Screenshot / GIF / MP4 with WGC backend

---

## 🍎 macOS (experimental — **not yet tested by the maintainer**)

An experimental macOS build is now available:

[**▶ Download GifCam-1.3.0-mac.dmg (prerelease)**](https://github.com/kuoungseok/gifcam/releases/tag/v1.3.0-mac.2)

> ⚠️ **Warning — this build has never been run on a real Mac.** It was
> authored entirely from Windows against Apple's API docs and built by
> GitHub Actions. The maintainer has not downloaded, installed, or
> launched the resulting `.app` on macOS even once. If it crashes, fails
> to open, or misbehaves, please [open an issue](https://github.com/kuoungseok/gifcam/issues)
> with the exact error — fixes land in new prerelease tags as they're
> diagnosed.

- **Requires** macOS 12.3 Monterey or newer · Apple Silicon (arm64) only
- **First launch**: right-click `GifCam.app` → **Open** (ad-hoc signed,
  so Gatekeeper blocks a plain double-click the first time)
- **Screen Recording permission** must be granted on first capture,
  then quit & relaunch

Source and build internals: [`mac/`](https://github.com/kuoungseok/gifcam/tree/main/mac) · [`mac/README-mac.md`](https://github.com/kuoungseok/gifcam/blob/main/mac/README-mac.md).

---

## Author

**KyoungSeok Ko** ([@kuoungseok](https://github.com/kuoungseok))

Built in Korea. Used at work every day.

## License

[MIT](LICENSE)
