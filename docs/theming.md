# Theming

DriftWM offers extensive theming options through `~/.config/driftwm/config.toml`. This page documents the key theming settings used in this setup.

## 🖼️ Wallpaper

This setup uses a custom wallpaper with the built-in wallpaper background type:
```toml
[background]
type = "wallpaper"
path = "/home/wgparch/Pictures/ALNW/Bluespaceship.jpg"

Available Background Types

    default — Built-in dot-grid pattern
    shader — Procedural GLSL shader (scrolls with canvas)
    tile — Tiled image with optional mirror-fold
    wallpaper — Single image stretched to canvas
    none — No built-in background (use swaybg/swww instead)

🎨 Decorations
Window chrome is configured in the [decorations] section:

[decorations]
# bg_color = "#303030"           # Title bar background
# fg_color = "#FFFFFF"           # Title text color
# corner_radius = 10             # Rounded corners
# shadow = true                  # Drop shadow
# border_width = 0               # Border thickness
# border_color = "#303030"       # Unfocused border
# border_color_focused = "#303030"  # Focused border

Decoration Modes

    client — Client draws its own titlebar (CSD, default)
    server — DriftWM draws the titlebar (SSD)
    minimal — No titlebar, just shadow/corners/border
    none — No chrome at all

✨ Effects
Enable blur and other visual effects:
[effects]
blur_radius = 2                # Kawase blur passes
blur_strength = 1.1            # Per-pass spread
animate_blur_fps = 20          # Blur refresh rate

🎯 Rofi Theme
The application launcher uses a custom Rofi theme:

[keybindings]
"mod+d" = "exec rofi -show drun -theme /usr/share/rofi/themes/fancy.rasi"

🪟 Per-Window Rules
Apply custom theming to specific applications:
[[window_rules]]
app_id  = "kitty"
opacity = 0.85
blur    = true

[[window_rules]]
app_id           = "firefox"
corner_radius    = 15
border_width     = 2
border_color_focused = "#4a90e2"

🔄 Live Reloading
DriftWM supports live config reloading. After editing config.toml:
driftwm msg reload

