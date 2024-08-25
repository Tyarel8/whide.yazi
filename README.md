# whide.yazi

A plugin for [yazi](https://github.com/sxyazi/yazi) to hide/unhide files or folders in windows.

## Installation

```sh
ya pack -a 'Tyarel8/whide'
```

## Usage

Add this to your `keymap.toml`:

```toml
[manager]
prepend_keymap = [
  { on   = [ "'", "h" ], run  = "plugin whide --args='hide'", desc = "Hide files" },
  { on   = [ "'", "H" ], run  = "plugin whide --args='unhide'", desc = "Unhide files" },
  { on   = [ "'", "<A-h>" ], run  = "plugin whide --args='toggle'", desc = "Toggle hidden status" },
]
```

It will apply to all selected or hovered if there is no selection.



