# TypePrint — Interactive Typing Fingerprint Generator

**Date**: 2026-03-28
**Builder**: Claude Code (autonomous)

## Idea Source
- **Origin**: HN Show HN "VizTools" (16 free tools, no AI) + trending data visualization tools
- **URL**: https://news.ycombinator.com/show
- **Why this idea**: Typing tests are universally popular, but none generate a unique visual "fingerprint" of your typing patterns. Combines gamification with beautiful data visualization.
- **Selection Score**: novelty: 5/5, feasibility: 5/5, wow: 5/5, learning: 4/5, utility: 4/5 = 52/55

## What It Does
TypePrint is a browser-based typing analyzer that captures your natural typing patterns and generates a beautiful, unique visual fingerprint. It tracks keystroke timing, rhythm, key frequency, and finger usage to create a shareable "TypePrint" — part typing test, part generative art.

## Target User
Developers, writers, and anyone who types daily and is curious about their typing patterns. Perfect for sharing on social media.

## Core Features (MVP Scope)
1. **Typing Test** — Type a curated passage with real-time WPM/accuracy tracking
2. **Keyboard Heatmap** — Visual heatmap showing key frequency on an interactive keyboard
3. **Rhythm Waveform** — Timing between keystrokes visualized as a unique waveform
4. **Bigram Speed Chart** — Top 10 fastest and slowest key combinations
5. **Finger Distribution** — Pie/donut chart showing which fingers do the most work
6. **TypePrint Card** — Shareable summary card with all visualizations combined

## Tech Stack
- **Frontend**: Single HTML + CSS + vanilla JavaScript (Canvas API for visualizations)
- **Backend**: None (100% client-side)
- **Database**: None
- **External APIs**: None
- **Deployment**: Vercel static

## UI Wireframe (text-based)
```
┌─────────────────────────────────────────────┐
│  TypePrint 🔤                    [About]     │
├─────────────────────────────────────────────┤
│                                             │
│  ┌─ Typing Area ──────────────────────┐     │
│  │ The quick brown fox jumps over...  │     │
│  │ [cursor blinks here]              │     │
│  └────────────────────────────────────┘     │
│                                             │
│  WPM: 72  |  Accuracy: 96%  |  Time: 45s   │
│                                             │
├─────────── Results (after typing) ──────────┤
│                                             │
│  ┌─ Keyboard Heatmap ─┐ ┌─ Rhythm Wave ─┐  │
│  │ [QWERTY keyboard]  │ │ [waveform]    │  │
│  │ [color-coded keys] │ │ [visualization│  │
│  └────────────────────┘ └───────────────┘  │
│                                             │
│  ┌─ Bigram Speeds ────┐ ┌─ Finger Use ──┐  │
│  │ [bar chart]        │ │ [donut chart] │  │
│  │ fastest/slowest    │ │ [per finger]  │  │
│  └────────────────────┘ └───────────────┘  │
│                                             │
│  ┌─ TypePrint Card ───────────────────┐     │
│  │ [Combined visualization summary]  │     │
│  │ [Share / Download button]         │     │
│  └────────────────────────────────────┘     │
│                                             │
└─────────────────────────────────────────────┘
```

## Success Criteria
- [x] App runs locally with one command (just open HTML)
- [ ] Core feature works end-to-end
- [ ] Beautiful dark-mode UI
- [ ] Keyboard heatmap renders correctly
- [ ] Rhythm waveform is visually interesting
- [ ] Shareable TypePrint card generation
- [ ] README with description
- [ ] Deployed on Vercel

## Out of Scope (save for v2)
- User accounts / saving history
- Multiplayer race mode
- Custom text passages
- Mobile keyboard support

## Risks & Mitigations
- **Risk**: Canvas rendering performance with many data points
  **Mitigation**: Limit data capture to reasonable intervals, use requestAnimationFrame
- **Risk**: Keyboard layout differences (AZERTY, etc.)
  **Mitigation**: Default to QWERTY with a note about layout assumption
