# GifCam

<p align="center">
  <b>Free Windows screen recorder — speed up the boring parts, slow down the important ones, draw, caption, and bubble-talk on your video. All in the same clip.</b>
</p>

<p align="center">
  <i>Screenshot · GIF · MP4 · Pro video editor — no watermark, no trial, no signup.</i>
</p>

<p align="center">
  <a href="https://github.com/kuoungseok/gifcam/releases/latest">
    <b>▶ Download the latest installer</b>
  </a>
</p>

---

## Screenshots

### Main window
<p align="center">
  <img src="docs/screenshots/main-window.png" alt="GifCam main window" width="520">
</p>

Win11 Snipping-Tool–style interface in a new dark theme. Pick a mode
(Screenshot / GIF / Video), hit **New capture**, then drag to select a
region. The **violet Open pro video editor** button is a one-click entry
to the full multi-track editor.

### Pro video editor
<p align="center">
  <img src="docs/screenshots/video-editor.png" alt="Pro video editor with speed segments and fade actor" width="720">
</p>

Multi-track timeline with live thumbnails, **per-region speed from 0.25×
to 16×** (shown here with a **×16** and **×0.5** segment on two different
tracks), cut segments, playhead scrubbing, **drag-drop fade transition
actors**, and one-click MP4 export. Mouse wheel on the timeline zooms
horizontally.

### 🖌 Paint + 💬 speech bubbles *(placed from the paint dialog)*
<p align="center">
  <img src="docs/screenshots/paint-dialog.png" alt="Paint dialog with pen stroke and speech bubble" width="720">
</p>

Click the preview in the Pro editor to open a paint-style annotation
dialog. Pen, eraser, 8-color palette + custom picker, width & opacity,
and an **Add bubble** button that drops an editable speech bubble onto
the frame (type directly into it, toggle the tail left/right, drag to
move, resize from the bottom-right grip, delete with ✕). Strokes *and*
bubbles are **burned into the exported MP4** — no separate tool needed.

### Subtitles
<p align="center">
  <img src="docs/screenshots/subtitle-editor.png" alt="Subtitle editor over a multi-track timeline" width="720">
</p>

Add time-aligned captions; toggle the background box on (semi-transparent
pill) or off (outline + drop shadow). Burned into the exported MP4.

---

## What makes GifCam different

### ⚡ Per-segment speed control in the **same** video
Select any range on the track and dial it from **0.25× up to 16× speed**.
Keep the rest at normal 1× — or stack multiple speed segments back to
back. A tutorial can zip through setup at 4× then settle into 1× for the
key steps, all in one clip. **ScreenToGif and ShareX don't do this.
Snagit charges $63.**

### 🖌 Draw live on your video  *(rare — almost no free tool does this)*
Click the preview in the Pro editor and a paint dialog opens over the
current frame. Pen, eraser, palette + custom color, width and opacity.
Strokes stay visible during playback and burn into the exported MP4.

### 💬 Speech bubbles  *(new in 1.3)*
Drop rounded-rect callouts with a left / right tail straight onto the
preview. Type text inline, drag to reposition, resize from the grip.
Perfect for tutorials ("click here"), bug repros ("it crashes at this
step"), and meme-style commentary. Burned into the export.

### 🎬 Drag-drop fade transitions  *(new in 1.3)*
Grab the **Fade** card from the toolbar, drop it on the track at any
point. The width of the placed actor = fade duration. Drag the edges to
resize. Right-click the actor to switch between **Fade In / Fade Out /
In + Out**. Live preview shows the fade as you play.

### 🪟 Drag-to-capture in under 2 seconds
Open GifCam, pick Screenshot / GIF / Video, hit **New capture**, drag a
region. That's it. No modal wizards, no codec picker, no pre-roll
countdown unless you turn it on.

### 🎞 Layered multi-track playback
Stack multiple clips on independent lanes, drag each clip left or right
on the project timeline to align it. The top track plays by default;
cut regions fall through to the track beneath, and short tracks reveal
the one under them once they end. No timeline gaps.

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
- **Full dark theme** across every window
- **Multi-monitor, mixed-DPI aware** region selector *and* sub-monitor
  capture (fixed in 1.3)
- **GIF encoder** with per-frame adaptive palette (+ automatic `gifski` /
  `gifsicle` if installed)
- **MP4 (H.264)** export with per-segment speed, cuts, fades, paint
  overlays, speech bubbles, and subtitle burn-in
- **Mouse-wheel zoom** on both the GIF frame strip and the Pro timeline
- **Multi-language UI** — 한국어 · English · 日本語 · Deutsch
  (auto-detected from Windows locale, live switchable)
- **Keyboard shortcuts** — `Ctrl+Shift+N` new capture, `Ctrl+1/2/3` mode
  switch, `Ctrl+O` save folder, `Ctrl+,` settings
- **Safe overwrite** — export writes to a temp file then atomically
  replaces the destination (no more "file locked" corruption)
- **Installer** that registers in *Settings → Apps* for a normal Windows
  uninstall experience

## Install

1. Download **`GifCam-Setup-1.3.0.exe`** from the
   [**Releases** page](https://github.com/kuoungseok/gifcam/releases/latest)
2. Double-click and follow the wizard — no admin rights required
3. Installed to `%LOCALAPPDATA%\GifCam`, listed in *Settings → Apps*

Captured files live in `~/Videos/GifCam` by default.

## System requirements

- Windows 10 1903+ or Windows 11
- x64

## Why is this free?

I built GifCam because I got tired of ScreenToGif not having per-segment
speed control and Snagit costing $63. I make tutorials and bug repros
every week, and the exact tool I wanted didn't exist at any price I was
willing to pay — so I just shipped one.

It stays free. No watermark, no trial, no "Pro edition coming soon"
nagware. If it saves you time too, a few bucks keeps me motivated to
keep pushing updates.

&mdash; Kyoungseok

- **PayPal** — https://paypal.me/KyoungseokKo
- **Toss Bank** (KRW transfer) — `1001-5567-2524` 고경석

## Author

**KyoungSeok Ko** ([artmouse](https://github.com/kuoungseok))

## License

[MIT](LICENSE)
