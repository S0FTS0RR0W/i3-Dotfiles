# i3 Dotfiles for ThinkPad X220

My personal dotfiles repository containing a minimal, efficient i3 window manager configuration optimized for the ThinkPad X220, featuring a clean tiling workflow with integrated tools for productivity and aesthetics.

## Overview

This is my personal collection of dotfiles for a complete i3 desktop environment setup tailored to my ThinkPad X220. The configuration emphasizes keyboard-driven navigation, screen real estate efficiency, and a distraction-free workflow suited to my preferences and workflow.

## Components

### i3 Window Manager
The core tiling window manager providing keyboard-driven window management and workspace organization. Configuration includes custom keybindings and layout rules optimized for the X220's 1366x768 display.

### i3status
Status bar displaying system information (time, date, network, battery status, etc.) at the top of the screen. Perfect for monitoring battery life and connectivity on a laptop.

### Kitty Terminal Emulator
A GPU-based terminal emulator with support for multiple themes. Configured with the **3024 Night** color scheme for a comfortable dark theme and uses modern font rendering.

### Picom Compositor
Compositing manager providing smooth animations, window shadows, and transparency effects. Lightweight configuration suitable for the X220's integrated graphics.

### Rofi Application Launcher
Fast, customizable application launcher and menu system. Includes multiple color themes:
- Dracula (dracula_config1.rasi, dracula_config2.rasi)
- Gruvbox Dark Soft (gruvbox-dark-soft.rasi)
- 3024 Night (colors.rasi)

## Installation

1. Clone this repository to your dotfiles directory:
   ```bash
   git clone https://github.com/S0FTS0RR0W/i3-Dotfiles ~/.config/
   ```

2. Ensure required packages are installed:
   ```bash
   # On Debian/Ubuntu
   sudo apt install i3 i3status kitty picom rofi

   # On Fedora
   sudo dnf install i3 i3status kitty picom rofi
   ```

3. Start i3 from your login manager or by running:
   ```bash
   startx ~/.xinitrc  # if configured for i3
   ```

## Configuration Structure

```
├── i3/                    # Main i3 window manager config
├── i3status/              # Status bar configuration
├── kitty/                 # Terminal emulator config and themes
├── picom/                 # Compositor configuration
└── rofi/                  # Application launcher themes and config
```

## Hardware Optimizations

This configuration is optimized for the **ThinkPad X220**:

- **Display**: 1366x768 resolution with efficient window tiling
- **Battery**: i3status monitors and displays battery percentage and charging status
- **Keyboard**: Leverages ThinkPad's excellent keyboard with custom keybindings
- **Performance**: Lightweight compositor and terminal emulator minimize resource usage
- **Touchpad**: Configured for efficient single-monitor productivity

## Quick Start

- **Mod Key**: Alt (customizable in i3 config)
- **Launch Applications**: Mod + Space
- **Terminal**: Mod + Return (opens Kitty)
- **Full Window Cycle**: Mod + Tab
- **Workspaces**: Mod + 1-9

For a complete list of keybindings, see the i3 config file.

## Theme Selection

Rofi and Kitty include multiple color schemes. To switch themes:

1. **Kitty**: Edit `kitty/kitty.conf` and reference different `*.conf` files
2. **Rofi**: Edit `rofi/config.rasi` to include your preferred color theme

## Customization

Feel free to modify any configuration to suit your preferences:
- Adjust i3 keybindings for your workflow
- Switch color schemes in Rofi and Kitty
- Fine-tune picom animations and effects
- Modify i3status information display

## Requirements

- i3 window manager
- i3status
- Kitty terminal
- Picom compositor
- Rofi launcher
- X11 session

## License

Feel free to use, modify, and distribute as needed.
