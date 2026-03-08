# fsr-minipad-obs-overlay

An OBS browser source overlay that visualizes [Rhythm Technologies FSR Mini Pad](https://rhythmtechnologies.net) inputs in real time. Includes two visual styles, each with a built-in settings page for customizing panel colors and input mapping.

---

## Overlays

### `FSR Mini Pad Overlay`
Detailed overlay modeled after the Rhythm Technologies FSR Mini Pad, complete with LED PCBs, brushed metal texture, and corner screws.

![FSR Mini Pad Overlay](Preview%20images/preview_minipad.png)

---

### `Simple Pad Overlay`
A clean, minimal alternative with the same functionality.

![Standard Overlay](Preview%20images/preview_standard.png)

---

## Setup

1. In OBS, add a **Browser Source**
2. Check **Local File** and select your chosen `.html` file
3. Set the width and height to **512×512**
4. Ensure your dance pad is connected before launching OBS

---

## Configuration

Both overlays include a built-in settings page. To open it, add `?settings` to the end of the file path in your browser:

```
file:///C:/path/to/fsr_minipad_overlay_v2.html?settings
```

> The settings page is intentionally hidden from OBS. OBS loads the plain file path with no query string, so it will always show the overlay only.

### Panel Colors

Each arrow panel has its own color picker. The default colors match the ITG2 dedicab arrow panels: **red** for left/right, **blue** for up/down.

### Input Mapping

Button numbers can vary between setups, so input mapping is left **unassigned by default**. To assign a button to a direction:

1. Open the settings page in your browser
2. Click **Assign** next to the direction you want to map
3. Press the corresponding button on your pad — it will be detected automatically
4. Repeat for all four directions
5. Click **Save**

Until all directions are assigned and saved, the overlay will not respond to any input.

### Saving & Resetting

- **Save:** writes your current colors and input mapping to the browser's local storage. Remember to reload the browser source in OBS after saving.
- **Reset to defaults:** clears all saved settings and restores the ITG2 default colors and empties input mappings.

---

## Requirements

- OBS Studio with Browser Source support
- A gamepad/controller recognized by the browser Gamepad API (such as the Rhythm Technologies FSR Mini Pad)

---

*Made with ❤️ by [playtagg](https://github.com/playtagg)*
