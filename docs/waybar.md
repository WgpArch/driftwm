# Waybar Configuration

This setup uses a custom Waybar configuration located at `~/.config/waybar4/`, launched automatically via DriftWM's autostart.

## 📂 File Structure

~/.config/waybar4/
├── config.jsonc   # Module layout and behavior
└── style.css      # Visual styling (colors, fonts, spacing)


## 🚀 Autostart Integration

Waybar is launched automatically by DriftWM. In `~/.config/driftwm/config.toml`, the `autostart` array includes:
```toml
autostart = [
  "/usr/lib/xdg-desktop-portal-gtk",
  "/usr/lib/xdg-desktop-portal",
  "waybar -c /home/wgparch/.config/waybar4/config.jsonc -s /home/wgparch/.config/waybar4/style.css",
  "nm-applet --indicator"
]

🎨 Modules Included
The configuration includes the following modules:

    Clock — Date and time display
    System Tray — Network manager and other tray icons
    Battery — Power status (for laptops)
    Network — Connection status
    Audio — Volume control via PipeWire/PulseAudio
    Workspaces — Spatial canvas bookmark indicators


🛠️ Customization
Editing the Layout
Open ~/.config/waybar4/config.jsonc to add, remove, or rearrange modules.
Styling
Open ~/.config/waybar4/style.css to change:

    Colors (background, text, borders)
    Font families and sizes
    Padding and margins
    Hover effects

Reloading
After making changes, reload Waybar without restarting DriftWM:
killall waybar && waybar -c ~/.config/waybar4/config.jsonc -s ~/.config/waybar4/style.css &
