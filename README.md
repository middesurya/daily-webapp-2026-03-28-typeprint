# TypePrint — Your Typing Fingerprint ⌨️

> Discover your unique keystroke DNA. An interactive typing analyzer that visualizes your rhythm, speed patterns, and finger habits beautifully.

![TypePrint](https://img.shields.io/badge/daily--webapp-2026--03--28-6c5ce7?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![AI Built](https://img.shields.io/badge/built%20with-Claude%20Code-a855f7?style=flat-square)

## 🔗 Live Demo

**[typeprint.vercel.app](https://daily-webapp-2026-03-28-typeprint.vercel.app)**

## What is TypePrint?

TypePrint is a browser-based typing analyzer that goes beyond simple WPM testing. It captures your natural typing patterns and generates a beautiful, unique visual "fingerprint" of how you type.

### Features

- **Real-time Typing Test** — Type a curated passage with live WPM and accuracy tracking
- **Keyboard Heatmap** — See which keys you press most on an interactive color-coded keyboard
- **Rhythm Waveform** — Your keystroke timing visualized as a unique waveform pattern
- **Key Pair Speeds** — Discover your fastest and slowest two-key combinations (bigrams)
- **Finger Distribution** — Breakdown of which fingers do the most work
- **TypePrint Card** — A shareable summary combining all your typing visualizations
- **Download** — Save your TypePrint as a PNG image

### Tech Stack

- **Frontend**: Single HTML file with vanilla JavaScript
- **Styling**: Custom CSS with CSS variables (dark mode)
- **Visualizations**: Canvas API
- **Dependencies**: Zero — no frameworks, no build step, no APIs
- **Deployment**: Vercel static hosting

## Getting Started

Just open `index.html` in your browser. That's it!

```bash
# Or serve with any static server
npx serve .
```

## How It Works

1. Click the typing area and start typing the displayed passage
2. TypePrint captures every keystroke timing in milliseconds
3. When finished, it analyzes your data and generates visualizations:
   - **Heatmap**: Key frequency mapped to color intensity
   - **Rhythm**: Time intervals between keystrokes as a waveform
   - **Bigrams**: Average speed for every two-key combination
   - **Fingers**: Which fingers type the most based on QWERTY layout
4. Download your unique TypePrint as a shareable image

## Daily Webapp Project

This is part of the **Daily Webapp** series — a new production-ready webapp built autonomously every day.

- **Day**: 2026-03-28
- **Idea Source**: HN Show HN trending tools + data visualization trend
- **Build Time**: Autonomous single-session build

## License

MIT — Use it however you like.

---

Built by [Surya Midde](https://github.com/middesurya) with Claude Code
