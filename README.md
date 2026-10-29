# spork apps drawer

GUI apps for [spork](https://github.com/spork-pm/spork), the macOS package manager that needs no admin rights.

spork's installer adds this drawer for you. To add it by hand:

```bash
spork drawer add apps https://github.com/spork-pm/apps
```

## Packages

| Package | Description |
|---|---|
| `headlamp` | A Kubernetes web UI that is fully-featured, user-friendly and extensible |
| `intellij` | Cross-Platform IDE for Java by JetBrains |
| `monitor-control` | Control your display's brightness & volume on your Mac as if it was a native Apple Display |
| `openlogi` | Remap Logitech mouse buttons, DPI and SmartShift without Logitech Options+ (no account, no telemetry) |
| `rectangle` | Move and resize windows with keyboard shortcuts and snap areas |
| `rider` | Cross-Platform IDE for .NET by JetBrains |
| `stats` | macOS system monitor in your menu bar (open source alternative to iStat Menus) |

## Adding a package

Add one JSON manifest per package in [drawer/](drawer/), named after the package (`drawer/<name>.json`).
This drawer is for GUI apps (anything installed into ~/Applications). Command-line tools go in [main](https://github.com/spork-pm/main). The manifest format is described in
[spork's README](https://github.com/spork-pm/spork#manifest-format). Get checksums with `spork hash <url>`, and test
with `spork install ./drawer/<name>.json` before opening a pull request.
