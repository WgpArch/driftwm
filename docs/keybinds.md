# Keybinds Reference

This page documents all custom keybindings configured in `~/.config/driftwm/config.toml`. The default modifier key is `Super` (the Windows/Cmd key).

## 🚀 Essentials
| Keybind | Action |
| :--- | :--- |
| `Super + Return` | Open default terminal |
| `Super + D` | Open Rofi application launcher (`fancy.rasi` theme) |
| `Super + Q` | Close focused window |
| `Super + F` | Toggle fullscreen for focused window |
| `Super + M` | Fit focused window to viewport |

## 📸 Screenshots & Navigation
| Keybind | Action |
| :--- | :--- |
| `Print Screen` | Take screenshot (saves to `~/Pictures/Screenshots/driftwm/`) |
| `Super + Down` | Center nearest window (down) |
| `Super + Left` | Center nearest window (left) |
| `Super + Right` | Center nearest window (right) |
| `Super + Shift + Up` | Nudge window up |
| `Super + Shift + Down` | Nudge window down |
| `Super + Shift + Left` | Nudge window left |
| `Super + Shift + Right` | Nudge window right |

## 🗺️ Spatial Canvas Bookmarks (11 Zones)
DriftWM uses an infinite canvas. These keybinds jump the camera to predefined spatial coordinates, acting like traditional workspaces.

### Top Row (Y = 3000)
| Keybind | Coordinates |
| :--- | :--- |
| `Super + 1` | `-4500, 3000` |
| `Super + 2` | `-1500, 3000` |
| `Super + 3` | `1500, 3000` |
| `Super + 4` | `4500, 3000` |

### Middle Row (Y = 0)
| Keybind | Coordinates |
| :--- | :--- |
| `Super + 5` | `-4500, 0` |
| `Super + 6` | `-1500, 0` |
| `Super + 7` | `1500, 0` |
| `Super + 8` | `4500, 0` |

### Bottom Row (Y = -3000)
| Keybind | Coordinates |
| :--- | :--- |
| `Super + 9` | `-4500, -3000` |
| `Super + 0` | `-1500, -3000` |
| `Super + -` | `1500, -3000` |
| `Super + =` | `4500, -3000` |
| `Super + [` | `6000, -3000` |

### 🏠 Home
| Keybind | Action |
| :--- | :--- |
| `Super + Space` | Toggle return to the center origin (`home-toggle`) |
