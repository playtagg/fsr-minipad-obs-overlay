# fsr-minipad-obs-overlay

An OBS browser source overlay that visualizes FSR Mini Pad inputs in real time. Includes two visual styles: a detailed overlay inspired by the design of the [Rhythm Technologies FSR Mini Pad](https://rhythmtechnologies.net), and a clean minimal alternative.

---

## Overlays

### `fsr_minipad_overlay.html`
Detailed overlay modeled after the Rhythm Technologies FSR Mini Pad, complete with FSRs, LED PCBs, brushed metal texture, and corner screws on each panel. For now the up and down panels will turn pink when pressed and the left and right panels will turn blue. This might be updated in the future to allow custom colours.

![FSR Mini Pad Overlay](Preview%20images/preview_minipad.png)

---

### `fsr_overlay_simple.html`
A plain, minimal alternative with the same input functionality. Panels will light up blue when pressed.

![Standard Overlay](Preview%20images/preview_standard.png)

---


## Setup Guide

1. In OBS, add a **Browser Source**
2. Check **Local File** and select your chosen `.html` file
3. Set the width and height to **512×512**
4. 

## Input Mapping

This is based on how the input mapping looked like for my minipad (if yours differs then you need to find out which sensor corresponds to which buttonn and change the corresponding values in the HTML files)

| Button | Direction |
|--------|-----------|
| B0 | Left |
| B1 | Right |
| B2 | Down |
| B3 | Up |

## Requirements

- OBS Studio with Browser Source support
- A gamepad/controller recognized by the browser Gamepad API (Has only been tested with the Rhythm Technologies FSR Mini Pad but I assume this should also work with other pads as long as they can be read by the gamepad api)
