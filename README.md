# fsr-minipad-obs-overlay

An OBS browser source overlay that visualizes FSR Mini Pad inputs in real time. Includes two visual styles: a detailed overlay inspired by the design of the [Rhythm Technologies FSR Mini Pad](https://rhythmtechnologies.net), and a clean minimal alternative.

---

## Overlays

### `fsr_minipad_overlay.html`
Detailed overlay modeled after the Rhythm Technologies FSR Mini Pad, complete with LED PCBs, brushed metal texture, and corner screws.

![FSR Mini Pad Overlay](Preview%20images/preview_minipad.png)

---

### `fsr_overlay_simple.html`
A plain, minimal alternative with the same input functionality.

![Standard Overlay](Preview%20images/preview_standard.png)

---


## Setup

1. In OBS, add a **Browser Source**
2. Check **Local File** and select your chosen `.html` file
3. Set the width and height to **512×512**
4. Ensure your dance pad is connected before launching OBS

## Input Mapping

| Button | Direction |
|--------|-----------|
| B0 | Left |
| B1 | Right |
| B2 | Down |
| B3 | Up |

## Requirements

- OBS Studio with Browser Source support
- A gamepad/controller recognized by the browser Gamepad API (such as the Rhythm Technologies FSR Mini Pad)
