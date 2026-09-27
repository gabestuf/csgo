# Gabe's CSGO Config

## CS2

Everything CS2 uses lives in `cs2/`. Copy all of its `.cfg` files into the game's cfg folder:

- Windows: `steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg`
- Linux: `~/.local/share/Steam/steamapps/common/Counter-Strike Global Offensive/game/csgo/cfg`

| File | What it does |
|---|---|
| `autoexec.cfg` | Main config: settings, binds, and aliases. Loads `crosshair1` and `nulls` |
| `crosshair1.cfg` | Main crosshair |
| `crosshair2.cfg` | `crosshair1` with a black outline |
| `crosshair3.cfg`–`crosshair11.cfg` | Extra crosshairs, from usable to ridiculous |
| `viewmodel1.cfg`–`viewmodel3.cfg` | Viewmodel presets |
| `nulls.cfg` | Null binds for A/D (used by the autoexec) |
| `nadeprac.cfg` | Nade practice server settings |
| `OtherSettings.md` | NVIDIA and other settings outside the game |

### Crosshair binds

| Key | Action |
|---|---|
| `8` | Toggle `crosshair1` / `crosshair2` (outline on/off) |
| `9` | Cycle `crosshair3` → `crosshair11` (prints the name in console) |
| `0` | Cycle crosshair color: red → green → cyan → yellow |
| `5` | Nade lineup crosshair (max-length lines), press again to go back |

The crosshair files use the cvars from the Sept 2026 "Rush Hour" update (`cl_crosshair_length`, `cl_crosshair_gap`, `cl_crosshair_thickness`, `cl_crosshaircolor_r/g/b/a`). Sizes are in pixels at `cl_crosshair_screen_height` and the game rescales them for other resolutions. `cl_crosshair_length` maxes out at 255.

### How 2 Exec

All config files can be executed by typing `exec nameoffile` in game console. (The file executed in this example would be `nameoffile.cfg`)

### To exec at launch:

1. Go to steam library and right click CS2 > Properties > General
2. Under launch options in the text field, add `+exec autoexec.cfg`

## CS:GO

`csgo (rip)/` has the old CS:GO config, kept for history.
