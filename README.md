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
| `rectangle` | Move and resize windows with keyboard shortcuts and snap areas |

## Adding a package

Add one JSON manifest per package in [drawer/](drawer/), named after the package (`drawer/<name>.json`).
This drawer is for GUI apps (anything installed into ~/Applications). Command-line tools go in [main](https://github.com/spork-pm/main). The manifest format is described in
[spork's README](https://github.com/spork-pm/spork#manifest-format). Get checksums with `spork hash <url>`, and test
with `spork install ./drawer/<name>.json` before opening a pull request.
