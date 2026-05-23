# Blender Launcher V2 - Flatpak

Unofficial Flatpak manifest for [Blender Launcher V2](https://github.com/Victor-IX/Blender-Launcher-V2).

> **Requirements:** x86_64 Linux with Flatpak. Does not support ARM.

## Build & Install

```bash
# Install flatpak-builder
sudo pacman -S flatpak-builder  # Arch/CachyOS
# or
sudo apt install flatpak-builder  # Ubuntu/Debian

# Install runtime
flatpak install flathub org.freedesktop.Platform//24.08 org.freedesktop.Sdk//24.08

# Download source zips
curl -L "https://github.com/Victor-IX/Blender-Launcher-V2/releases/download/v2.6.1/Blender_Launcher_v2.6.1_Ubuntu_x64.zip" -o blender-launcher-ubuntu.zip
curl -L "https://github.com/Victor-IX/Blender-Launcher-V2/releases/download/v2.6.1/Blender_Launcher_v2.6.1_Linux_x64.zip" -o blender-launcher.zip

# Build and install
flatpak-builder --user --install --force-clean build io.github.VictorIX.BlenderLauncherV2.yml

# Run
flatpak run io.github.VictorIX.BlenderLauncherV2
```
