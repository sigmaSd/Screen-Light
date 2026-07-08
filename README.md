# Screen Light

A GTK4 GUI tool to adjust external monitor brightness via DDC/CI, built with
Deno.

## Requirements

- Linux with `ddccontrol` service running:
  ```
  sudo systemctl start ddccontrol
  ```
- Deno

## Install

```
deno task install
```

This compiles the binary and installs it with a `.desktop` shortcut and icon.

## Run

After install, launch **Screen Light** from your app menu, or run:

```
~/.local/share/deno-installed-apps/Screen_Light/Screen_Light
```

Or directly from the repo:

```
deno run -A main.ts
```

## Development

```bash
# compile only
deno task compile

# compile and install
deno task install

# uninstall
deno run -A jsr:@sigmasd/install-app uninstall Screen_Light
```
