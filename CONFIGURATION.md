# Configuration guide

## Umbriel

`config.toml` contains the compositor configuration, including keyboard behavior and custom bindings. Check the comments in the file before adapting the bindings to a different keyboard or display setup.

`noctalia.toml` is the Umbriel-side integration configuration for the Noctalia shell/theme.

## Noctalia

`bar.toml` customizes the default bar layout, media widget sizing, transparency, and panel placement. The referenced Voxtype status widget requires its Noctalia widget/provider to be installed.

`templates.toml` and the files in `templates/` provide the local palette/template resources. The Umbriel palette file intentionally contains only the compatible color subset.

## Safe changes

1. Preserve a copy of your working config before making changes.
2. Validate TOML with a parser and check the installed app's documentation for supported settings.
3. Restart or reload the relevant application after applying updates.
