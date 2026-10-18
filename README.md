# run-raise-cli

A shell script wrapper around the [run-or-raise](https://github.com/e2m/run-or-raise) GNOME extension's D-Bus interface, so you can invoke it from keyboard shortcuts without maintaining a config file.

## Requirements

- [run-or-raise](https://github.com/e2m/run-or-raise) extension installed and enabled
- D-Bus enabled in the extension settings (via the Extensions app or GNOME Tweaks), then disable and re-enable the extension for it to take effect

## Installation

```
sudo curl -o /usr/local/bin/runraise https://raw.githubusercontent.com/dsrosen6/gnome-run-raise-script/main/runraise && sudo chmod +x /usr/local/bin/runraise
```

## Usage

```
runraise <command> [wm_class] [title]
```

```
runraise firefox
runraise gnome-terminal Gnome-terminal
```

Bind any of these as a GNOME keyboard shortcut command.
