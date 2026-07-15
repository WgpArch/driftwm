# Installation

This guide covers how to install DriftWM and deploy this specific configuration.

## 📦 Installing DriftWM

DriftWM is a Wayland compositor. Install it according to your distribution's package manager or build from source.

### Arch Linux
```bash
# Install from the AUR (if available) or build from source
trizen -S driftwm

Dependencies
Ensure you have the following installed:

    wayland — Wayland display server protocol
    wlroots — Modular Wayland compositor library
    grim — Screenshot utility (for the Print key binding)
    rofi-wayland — Application launcher
    waybar — Status bar
    xdg-desktop-portal-gtk — Desktop portal integration
    network-manager-applet — Network manager tray applet

git clone https://github.com/WgpArch/dotfiles.git ~/.dotfiles
cd ~/.dotfiles/driftwm
mkdir -p ~/.config/driftwm
cp configs/driftwm/config.toml ~/.config/driftwm/
mkdir -p ~/.config/driftwm/rofi
mkdir -p ~/.config/driftwm/screenshots
cp docs/screenshots/* ~/.config/driftwm/screenshots/
cp docs/rofi/* ~/.config/driftwm/rofi/
mkdir -p ~/.config/waybar4
cp configs/waybar/* ~/.config/waybar4/
driftwm --check-config

Via Display Manager
If you have a display manager (GDM, SDDM, LightDM), select "DriftWM" from the session list after installing the .desktop file.
✅ Post-Installation
After your first login:

    Verify the "Bluespaceship" wallpaper loads
    Test Super + D to open Rofi
    Press Print Screen to take a screenshot (saved to ~/Pictures/Screenshots/driftwm/)
    Try the spatial bookmarks with Super + 1 through Super + =
