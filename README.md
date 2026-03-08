<<<<<<< HEAD
# 🖥️ PocketDesk

> **A full desktop experience from your iPhone — no Mac, no PC, no iPad required.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-Ready-green.svg)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
[![Works on iOS](https://img.shields.io/badge/iOS-16%2B-black.svg)](https://www.apple.com/ios)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Mac%20%7C%20Linux-lightgrey.svg)](#desktop-companion-app)

---

## Why PocketDesk exists

Not everyone can afford a Mac, PC, laptop, or iPad.

But a lot of people already have an iPhone — and keyboards, mice, and monitors are cheap. A used mechanical keyboard runs $20. A monitor is $80 at a garage sale. An HDMI adapter is $15.

**PocketDesk turns that $115 setup into a real desktop computer.**

No jailbreak. No hacks. No subscription. Just your iPhone, a monitor, and a cable.

---

## What it does

Connect your iPhone to a monitor via HDMI adapter, pair a Bluetooth keyboard and mouse, and PocketDesk gives you:

| Feature | Description |
|---|---|
| 🌐 **Browser** | Full web browser with address bar and navigation |
| 📝 **Notes** | Multi-note editor with sidebar |
| 📁 **Files** | iCloud Drive file explorer |
| 🎵 **Music** | Player with iOS Media Session controls |
| 🔢 **Calculator** | Full scientific-style calculator |
| ⬛ **Terminal** | Simulated terminal with real commands |
| 🕐 **Clock** | Live clock and date |
| ⚙️ **Settings** | Mouse/keyboard detection, display info |
| 🖼️ **Wallpapers** | 8 built-in wallpaper themes |
| ⌨️ **Keyboard shortcuts** | Cmd+B (Browser), Cmd+N (Notes), Cmd+T (Terminal), Cmd+W (Close) |

All windows are **draggable**, **resizable**, and **multi-instance**. Right-click the desktop for the context menu.

---

## Hardware you need

| Item | Approx. Cost |
|---|---|
| Lightning → HDMI adapter (iPhone 14 and older) | $10–$20 |
| USB-C → HDMI adapter (iPhone 15+) | $10–$15 |
| Any HDMI monitor or TV | $0 (reuse old one) |
| Bluetooth keyboard | $15–$30 |
| Bluetooth mouse | $10–$20 |
| **Total** | **~$35–$85** |

---

## Quickstart

### Option A — Use it instantly (hosted)

> Coming soon: `pocketdesk.app`

### Option B — Run it yourself (2 minutes)

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/pocketdesk.git
cd pocketdesk

# 2. Serve it locally (any static server works)
npx serve .

# 3. Open on your iPhone
# Visit http://YOUR_LOCAL_IP:3000 in Safari
```

### Option C — Deploy free to GitHub Pages

```bash
# Push to main branch, then enable GitHub Pages in repo Settings
# Your URL: https://yourusername.github.io/pocketdesk
```

### Option D — Deploy free to Netlify / Vercel

Drag the `pocketdesk/` folder onto [netlify.com/drop](https://netlify.com/drop) — done in 30 seconds.

---

## Install as PWA (recommended)

For the best experience, install PocketDesk as a PWA so it launches fullscreen:

1. Open the URL in **Safari** on your iPhone
2. Tap the **Share** button → **Add to Home Screen**
3. Tap **Add**
4. Launch from your home screen — it opens fullscreen

When connected to your monitor, the desktop UI launches automatically on the external display.

---

## Desktop Companion App

PocketDesk also includes an **Electron companion app** for Windows, Mac, and Linux that adds:

- AirPlay device discovery (wireless iPhone mirroring via UxPlay)
- USB iPhone detection (via libimobiledevice)
- Native desktop shell with dock and menu bar

```bash
cd electron-app
npm install
npm start

# Build for your platform:
npm run build:win    # Windows .exe
npm run build:mac    # macOS .dmg
npm run build:linux  # Linux .AppImage
```

See [electron-app/README.md](electron-app/README.md) for full setup instructions including AirPlay and USB mirroring.

---

## How external display detection works

iOS 16+ outputs the browser to an external display when connected via HDMI adapter. PocketDesk detects this automatically by comparing `window.screen` dimensions to `window.innerWidth` — when they differ significantly, it switches to desktop mode.

```javascript
const isExternal = window.screen.width > window.innerWidth * 1.2
  || window.innerWidth >= 900;
```

On your iPhone screen, you'll see the connection guide. On the monitor, the full desktop launches.

---

## Project structure

```
pocketdesk/
├── index.html          # Main PWA — the full desktop shell
├── manifest.json       # PWA manifest (installable, fullscreen)
├── sw.js               # Service worker (offline support)
├── electron-app/       # Cross-platform desktop companion
│   ├── main.js         # Electron main process
│   ├── preload.js      # Secure IPC bridge
│   ├── index.html      # Electron UI
│   └── package.json    # Build config
├── LICENSE             # MIT License
├── .gitignore
└── README.md
```

---

## Roadmap

- [ ] Hosted version at `pocketdesk.app`
- [ ] Proxy layer for unrestricted browser (bypass iframe restrictions)
- [ ] File upload/download support
- [ ] App store (launch deep-links to installed iOS apps)
- [ ] Multiple desktops / virtual workspaces
- [ ] Theming system
- [ ] iOS Shortcuts integration
- [ ] Community wallpaper packs

---

## Contributing

Pull requests are welcome. For major changes, open an issue first.

This project exists to make computing more accessible. Please keep that mission in mind.

```bash
git clone https://github.com/yourusername/pocketdesk.git
git checkout -b feature/your-feature
git commit -m "Add your feature"
git push origin feature/your-feature
# Open a pull request
```

---

## License

[MIT](LICENSE) — free forever. Use it, build on it, share it.

---

## Credits

Built with the belief that computing should be accessible to everyone — not just people who can afford a $1,000 Mac.

If this helped you or someone you know, drop a ⭐ on GitHub. It helps more people find it.

---

<div align="center">
  <sub>Made with 📱 + ❤️ for people who deserve a desktop</sub>
</div>
=======
# pocketdesk
practice files
>>>>>>> 39b6ef6cc5ca3264b935bc0069ab137889e94d4e
