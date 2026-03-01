# NoRecoil v2

A sleek recoil compensation overlay for Rainbow Six Siege with a modern neon-styled UI.

Built on top of [Halqq's NoRecoil-Macro](https://github.com/Halqq/NoRecoil-Macro) — the original foundation. This version is a full rework of the interface, adds new features, and improves the overall experience.

PREVIEW:
https://streamable.com/e8w0n4

Join our DC to report issues:
https://discord.gg/dfPJjrSUGU

---

## What's New in v2

- Completely redesigned UI with animated neon glow theme
- Persistent HUD overlay that stays visible at all times
- Window link system for screen-share setups
- Rebindable hotkeys with visual key prompts
- Fullscreen overlay (auto-detects your monitor resolution)
- Search bars in operator lists
- Per-slider color coding with glow effects
- Customizable accent color that applies across the entire UI

---

## Quick Start

1. Download the latest `discord.exe` from releases
2. Run as administrator
3. Right Shift opens the menu (rebindable)
4. Pick your operator, tweak the sliders, close the menu
5. Hold LMB + RMB in-game — recoil compensation kicks in

---

## Controls

| Key | Action |
|-----|--------|
| Right Shift | Toggle menu (rebindable) |
| Delete | Toggle macro on/off (rebindable) |
| Arrow Up/Down | Increase/decrease vertical recoil by 1 (live, no menu needed) |
| Insert | Lock/unlock arrow keys (prevents accidental recoil changes) |
| LMB + RMB | Activate compensation (while macro is on) |

**Arrow key adjustment:** You can change your vertical recoil strength on the fly without opening the menu — just press Arrow Up or Arrow Down. This is useful for fine-tuning mid-game. If you want to prevent accidental changes (e.g. while moving in-game), press Insert to lock the arrow keys. The HUD shows whether keys are currently FREE or LOCKED.

---

## Settings

Everything is in the **Settings** tab inside the overlay:

**Theme** — Pick any accent color. The entire UI adapts: particles, glows, sliders, borders, everything.

**Keybinds** — Click a keybind button, press any key, done.

**HUD Overlay** — The small always-on status display. Choose what to show (status, keys, operator) and where (any corner). Stays visible even with the menu closed.

**Window Link** — Dropdown with all open windows. Select one for Discord screen-share purposes. The overlay stays freely movable regardless.

---

## Config Files

Stored in `Documents\NoRecoil\`:

- `macro_config.json` — operator profiles, selected operators, macro state
- `app_config.json` — theme color, keybinds, HUD and overlay settings

Everything auto-saves. No manual editing needed.

---

## Building from Source

Requires .NET 8 SDK.

```bash
cd norecoil
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```

The output `.exe` is standalone — no runtime installation needed on the target machine.

---

## Credits

Original project by **[Halqq](https://github.com/Halqq/NoRecoil-Macro)**. This repo is a modified and extended version with a new UI, additional features, and quality-of-life improvements. All credit for the core macro logic goes to the original author.

---

## Disclaimer

Use at your own risk. This tool uses standard Windows input APIs and does not inject into or modify any game process. Check your game's terms of service before using.

MIT License — see [LICENSE](LICENSE).
