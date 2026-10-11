# ghostty-config

Personal [Ghostty](https://ghostty.org) configuration, originally converted from an iTerm2 profile.

## Contents

- `config`: main Ghostty config
- `themes/`: `iterm2-Default-light` and `iterm2-Default-dark` (theme follows system appearance)

## Install

```sh
# move any existing config aside first
mv ~/.config/ghostty ~/.config/ghostty.bak 2>/dev/null
git clone https://github.com/hernang87/ghostty-config.git ~/.config/ghostty
```

Then reload with `Cmd+Shift+,` (or restart Ghostty) and optionally check it with `ghostty +validate-config`.

## Requirements

- Fonts: Monaco (primary) and Menlo (fallback). Both ship with macOS; install them manually on other platforms or change `font-family`.
- Some options are macOS-only (`macos-titlebar-style`, `font-thicken`) and are ignored elsewhere.

## Notes

- The `scrollback-limit` is in bytes, estimated from the iTerm2 line count at ~160 bytes per line.
- Legacy character encodings from iTerm2 were not carried over (Ghostty is UTF-8).
