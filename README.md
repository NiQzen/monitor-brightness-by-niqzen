# Monitor Brightness for Stream Deck +

Control the brightness of your external monitors (DDC/CI) with the dials and touch strip of **Stream Deck +**.

| Control | Action |
|---|---|
| Rotate dial | Change brightness by the configured step (1–25 %) |
| Press dial / tap touch strip | Set brightness to 100 % |
| Hold dial / long-tap touch strip | Set brightness to 0 % |

## Settings (per dial)
- **Title** – label shown on the touch strip
- **Dial step** – percentage per click
- **Monitor #** – `0` = all DDC/CI monitors, `1`, `2`, … = a single monitor
- **Hold time** – how long to hold before brightness goes to 0 %

## Requirements
- Windows 10 / 11, Stream Deck 6.9 or later, Stream Deck +
- An external monitor with **DDC/CI enabled** in its on-screen menu. Some docks/adapters do not pass DDC/CI through. Features such as dynamic contrast / HDR modes can lock brightness.

## How it works
The plugin talks to the monitor through the Windows High-Level Monitor Configuration API (`dxva2.dll`) using a small PowerShell helper. No data leaves your computer.

## Support
Open an issue on the project page.
