# Monitor Brightness for Stream Deck

Control the brightness of your external monitors (DDC/CI) from Stream Deck keys and the dials of **Stream Deck +**.

**No Stream Deck + required:** the Brightness action works on every Stream Deck model with keys. On a Stream Deck + you can also use the dials and the touch strip.

## Setup
1. **Turn on DDC/CI on your monitor.** Open the monitor's on-screen menu with its buttons and enable the option called **DDC/CI** (often under *Setup*, *System* or *Others*). Many monitors have it on by default.
2. **Install the plugin** from the Elgato Marketplace. It appears in the Stream Deck app under **Monitor Brightness**.
3. **Add Brightness:** drag the **Brightness** action onto a key or, on a Stream Deck +, onto a dial.
4. **Pick the monitor:** in the action's settings, leave **Monitor #** at `0` to control all monitors together, or enter `1`, `2`, … to control one monitor. With several monitors, add one action per monitor.

**If the action shows a warning triangle**, the monitor did not answer:
- check that DDC/CI is on in the monitor's menu,
- connect the monitor directly (DisplayPort or HDMI); some docks and adapters do not pass DDC/CI through,
- turn off dynamic contrast, eco or HDR picture modes, which can lock brightness,
- check the **Monitor #** setting.

## Controls

**On a dial (Stream Deck +)**

| Control | Action |
|---|---|
| Rotate dial | Change brightness by the configured step (1–25 %) |
| Press dial / tap touch strip | Set brightness to 100 % |
| Hold dial / long-tap touch strip | Set brightness to 0 % |

**On a key**

| Control | Action |
|---|---|
| Press key | Set brightness to 100 % |
| Hold key | Set brightness to 0 % |

## Settings
- **Monitor #** – `0` = all DDC/CI monitors, `1`, `2`, … = a single monitor
- **Hold time** – how long to hold before brightness goes to 0 %
- **Title** – label shown on the touch strip (dial only; on a key, use Stream Deck's own title)
- **Dial step** – percentage per dial click (dial only)

## Requirements
- Windows 10 / 11, Stream Deck 6.9 or later
- Keys work on every Stream Deck with keys; dial features need a Stream Deck +
- An external monitor with **DDC/CI enabled** in its on-screen menu. Some docks/adapters do not pass DDC/CI through. Features such as dynamic contrast / HDR modes can lock brightness. Built-in laptop displays are not supported.

## How it works
The plugin talks to the monitor through the Windows High-Level Monitor Configuration API (`dxva2.dll`) using a small PowerShell helper. No data leaves your computer.

## Need more?
[Monitor Brightness Plus](https://github.com/NiQzen/monitor-brightness-plus-by-niqzen) adds more key actions (increase / decrease with hold to repeat, set a fixed level, cycle through levels), shows the current level on the key, and controls Windows **Night Light** from keys and dials, with an on/off schedule.

## Release notes

### 1.1.0
- **New: Brightness on keys.** The Brightness action now also works on keys, so the plugin works on every Stream Deck model, not just Stream Deck +.
- On a key: press for 100 %, hold for 0 %. Choose the monitor and the hold time in the action's settings.
- Existing dial setups keep working; nothing to change.

### 1.0.0
- First release: control monitor brightness with the dials and touch strip of Stream Deck +.

## Support
Open an issue on this page.
