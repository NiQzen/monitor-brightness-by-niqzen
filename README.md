# Monitor Brightness for Stream Deck

Control the brightness of your external monitors (DDC/CI) right from your Stream Deck.

Works on every Stream Deck model with keys. On a Stream Deck +, you can also use the dials and the touch strip.

## On a dial (Stream Deck +)
- **Rotate:** adjust brightness by a configurable step (1–25%)
- **Press or tap:** 100%
- **Hold or long-tap:** 0%

## On a key
- **Press:** 100%
- **Hold:** 0%

## Settings
- **Monitor #:** `0` controls all DDC/CI monitors together; enter `1`, `2`, … to control one monitor. With several monitors, add one action per monitor.
- **Hold time:** how long to hold before brightness goes to 0%
- **Title** and **Dial step** (dial only)

## Setup
1. Turn on **DDC/CI** in your monitor's on-screen menu (often under *Setup*, *System* or *Others*). Many monitors have it on by default.
2. Drag the **Brightness** action onto a key or a dial.
3. Pick the monitor in the action's settings.

If the action shows a warning triangle, the monitor did not answer. Check that DDC/CI is on, connect the monitor directly (some docks and adapters don't pass DDC/CI through), and turn off dynamic contrast, eco or HDR picture modes, which can lock brightness.

## Requirements
- Windows 10 / 11, Stream Deck 6.9 or later
- An external monitor with DDC/CI enabled. Built-in laptop displays are not supported.

No data leaves your computer.

## Need more?
[Monitor Brightness Plus](https://github.com/NiQzen/monitor-brightness-plus-by-niqzen) adds increase/decrease keys (hold to repeat), fixed levels, cycling through levels, the current level shown on the key, and Windows Night Light control on keys and dials.

## Release notes

### 1.1.0
- **New: Brightness on keys.** The Brightness action now also works on keys, so the plugin works on every Stream Deck model, not just Stream Deck +.
- On a key: press for 100%, hold for 0%. Choose the monitor and the hold time in the action's settings.
- Existing dial setups keep working; nothing to change.

### 1.0.0
- First release: control monitor brightness with the dials and touch strip of Stream Deck +.

## Support
Open an issue on this page.
