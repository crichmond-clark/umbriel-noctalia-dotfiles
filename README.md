# Umbriel + Noctalia dotfiles

Personal configuration for [Umbriel](https://github.com/umbriel-linux/umbriel) and [Noctalia](https://github.com/noctalia-dev/noctalia-shell). Files are kept under `.config/` so they map directly to their locations in `$HOME`.

## Contents

- `.config/umbriel/config.toml` — Umbriel compositor settings and keybindings.
- `.config/umbriel/noctalia.toml` — Umbriel integration/theme settings for Noctalia.
- `.config/noctalia/bar.toml` — Noctalia bar, widgets, and panel presentation.
- `.config/noctalia/templates.toml` and `templates/` — palette and template assets, including the Umbriel-compatible palette and Zen CSS.

## Install

Back up any existing files first, then from this repository root run:

```sh
cp -a .config/. "$HOME/.config/"
```

Log out and back in, or restart the relevant shell/compositor services, if needed. Review the configuration before applying it: keybindings and widget/plugin names may depend on your installed versions and extensions.

## Requirements and notes

- Umbriel and Noctalia installed and configured on your system.
- The bar configuration references the `gabedunn/voxtype:status` widget; install its provider or remove that entry if unavailable.
- These are personal settings, not a complete system setup. Packages, fonts, wallpapers, and machine-specific setup are not included.
- No backup copies or runtime state are tracked. Keep credentials and machine-specific secrets out of commits.

## Updating

Edit the files under `.config/`, commit the changes, and push them to your fork/repository. To update a machine, back up its existing configs and copy the tracked files into `~/.config/`.
