# Nine Workspaces

Keep workspace buttons **1–9** visible in the Omarchy top bar, including empty workspaces.

This is a copy of Omarchy’s workspace widget with one code change: the default button list has nine entries instead of five. Active workspace 10 still appears when present, matching upstream behavior. No new settings or background processes.

## Install

```sh
omarchy plugin add https://github.com/xi-void/omarchy-nine-workspaces --enable
```

This replaces the built-in workspace widget, preserving its position. The plugin ID is `qrzn.workspaces`; if you already have a local clone with that ID, back it up and resolve the existing directory before installing.

## Remove

```sh
omarchy plugin remove qrzn.workspaces
```

Removing the active clone restores the built-in workspace widget.

## Requirements

Omarchy Quattro with the Quickshell plugin system, Hyprland, and `hyprctl`. Uses Omarchy’s bundled QML components. No extra packages, network requests, install scripts, or elevated privileges.

## Credits and license

Derived from [Omarchy’s workspace widget](https://github.com/omacom/omarchy/blob/quattro/shell/plugins/bar/widgets/Workspaces.qml). Original code copyright David Heinemeier Hansson. Distributed under the upstream MIT license; see LICENSE.
