# GNOME UI Overrides

Custom CSS overrides for GNOME Shell, GTK3 and GTK4.

## Objective

This project aims to make GNOME visually more direct and less rounded, reducing excessive curvature and creating a cleaner, more compact interface.

The goal is not to redesign GNOME, but to refine it:

- Smaller border radius
- More consistent visual language
- Less “bubble-like” appearance
- Cleaner and more workstation-oriented aesthetics

## Scope

The overrides currently target:

- GNOME Shell (`gnome-shell.css`)
- GTK3 (`gtk-3.0/gtk.css`)
- GTK4 (`gtk-4.0/gtk.css`)

## Philosophy

This is not a theme.

It is a set of minimal CSS overrides applied on top of Adwaita, preserving GNOME’s design language while tightening its visual geometry.

The intent is subtle refinement, not radical transformation.

## Status

> ⚠ **Work in progress**.

This repository is actively evolving.
Selectors may change as GNOME versions evolve.
Values may be adjusted over time for consistency and balance.

## Compatibility

Designed and tested on:

- Fedora
- GNOME (recent versions)
- Wayland session

Behavior may vary across GNOME releases due to internal CSS changes.

## Installation

### GTK (Applications)

The folders:

- `gtk-3.0`
- `gtk-4.0`

must be copied to: `~/.config/`

Resulting in:

```sh
~/.config/gtk-3.0/gtk.css
~/.config/gtk-4.0/gtk.css
```

After copying, restart the affected applications. On Wayland sessions, a logout/login is required for changes to take effect.

### GNOME Shell

The `CompactShell` folder must be copied to `~/.themes/`.

Resulting in:

`~/.themes/CompactShell/gnome-shell/gnome-shell.css`

> Make sure the **User Themes** extension is enabled, then activate the theme using **Gnome Tweaks**.

## Disclaimer

GNOME Shell and libadwaita internals change frequently.
Future GNOME updates may require selector adjustments.

Use at your own discretion.
