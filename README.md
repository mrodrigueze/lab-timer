# 🧪 Lab Timer — Multi-Category Laboratory Timer

A lightweight, offline-ready web timer built for laboratory workflows that require precise, simultaneous timing of multiple samples across different reaction stages.

> Designed for colorimetric assay workflows where each sample must be read at an exact time point on a spectrophotometer after sequential reagent additions and homogenization steps.

---

## ✨ Features

- **Multiple simultaneous timers** — launch as many as needed, all running independently
- **Numbered timers per category** — each sample is tracked as #1, #2, #3... within its category
- **Custom categories** — rename, recolor, add or remove sample groups freely
- **Quick-launch buttons** — one-tap to start a preconfigured timer (e.g. 10 min, 5 min)
- **Audible alarm** — distinct chime when each timer reaches zero
- **Overtime display** — timer continues counting up (+) after expiry so you know how late a reading is
- **Global stopwatch** — sticky chronometer for total session tracking
- **Persistent configuration** — categories and buttons are saved to `localStorage`; your setup survives page reloads and browser restarts
- **Reset to defaults** — one-tap restore inside the settings modal
- **Zero dependencies** — single HTML file, no internet required, works offline

---

## 🔬 Use Case

This tool was built to support colorimetric assay protocols (e.g. Griess reaction for nitrite/nitrate quantification) where multiple samples are processed in sequence:

```
Sample workflow per replicate:
  1. Homogenization step       → start timer (e.g. 2 min)
  2. Add Reagent 1             → start timer (e.g. 5 min)
  3. Homogenization step       → start timer
  4. Add Reagent 2             → start timer
  5. Resting / color development → start timer (10 min)
  6. Read absorbance at spectrophotometer at exact time
```

With multiple samples running simultaneously, the numbered + color-coded timers make it immediately clear which sample needs attention next.

---

## 🚀 Getting Started

No installation required.

1. Download `index.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Configure your sample categories via the **⚙ settings** button
4. Add quick-launch buttons for your most common reaction times
5. Start timing

Your configuration is automatically saved and will be there next time you open the file.

---

## 🖥️ Interface Overview

| Element | Description |
|---|---|
| Top bar | Global stopwatch — tracks total session time |
| Category selector | Switch between sample groups |
| Quick buttons | One-tap timer launch for preset durations |
| Timer grid | Active timers — color-coded by category, numbered per group |
| ⚙ button | Open category editor — rename, recolor, add, remove |
| + button | Add a new quick-launch timer duration |

---

## ⚙️ Configuration

### Categories
- Each category represents a sample group (e.g. "Sample A", "Blank", "Standard")
- Assign a unique color per category for instant visual identification
- Changes are saved automatically

### Quick Buttons
- Preset durations for your most common reaction times
- Add via the **+** button, remove via the **✕** on each button
- Saved automatically between sessions

### Reset
- Open ⚙ → **Restore default configuration** to return to factory settings

---

## 🛠️ Tech Stack

- **HTML5 / CSS3 / Vanilla JavaScript** — no frameworks, no dependencies
- **Web Audio API** — procedural alarm sound generation
- **localStorage** — persistent configuration without a backend

---

## 📁 Project Structure

```
lab-timer/
└── index.html    # Complete application — single file
```

---

## 🔮 Planned Improvements

- [ ] Export timer log to CSV (timestamp per sample)
- [ ] Preset protocol templates (load a full workflow in one tap)
- [ ] PWA support (installable on mobile as standalone app)
- [ ] Vibration alert on mobile devices

---

## 👤 Author

**Manuel Isaias Rodriguez Espejo**  
Biotechnology Researcher · Universidad Nacional del Santa · Peru  
[GitHub](https://github.com/) · [LinkedIn](https://linkedin.com/)

---

## 📄 License

MIT — free to use, modify and distribute.
