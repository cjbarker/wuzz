# wuzz

Interactive cli tool for HTTP inspection

Wuzz command line arguments are similar to cURL's arguments,
so it can be used to inspect/modify requests copied from the
browser's network inspector with the "copy as cURL" feature.

![wuzz screencast](docs/images/screencast.gif)

## Installation and usage

```
$ go get github.com/asciimoo/wuzz
$ "$GOPATH/bin/wuzz" --help
```


### Configuration

It is possible to override default settings in a configuration file.
The default location is `"$XDG_CONFIG_HOME/wuzz/config.toml"`on linux
and `~/.wuzz/config.toml` on other platforms.
`-c`/`--config` switches can be used to load config file from custom location.

See [example configuration](sample-config.toml) for more details.


### Commands

Keybinding                              | Description
----------------------------------------|---------------------------------------
<kbd>F1</kbd>                           | Display help
<kbd>Ctrl+R</kbd>                       | Send request
<kbd>Ret</kbd>                          | Send request (only from URL view)
<kbd>Ctrl+S</kbd>                       | Save response
<kbd>Ctrl+Q</kbd>                       | Quit
<kbd>Ctrl+K</kbd>, <kbd>Shift+Tab</kbd> | Previous view
<kbd>Ctlr+J</kbd>, <kbd>Tab</kbd>       | Next view
<kbd>Alt+H</kbd>                        | Toggle history
<kbd>Down</kbd>                         | Move down one view line
<kbd>Up</kbd>                           | Move up one view line
<kbd>Page down</kbd>                    | Move down one view page
<kbd>Page up</kbd>                      | Move up one view page
<kbd>F2</kbd>                           | Jump to URL
<kbd>F3</kbd>                           | Jump to query parameters
<kbd>F4</kbd>                           | Jump to HTTP method
<kbd>F5</kbd>                           | Jump to request body
<kbd>F6</kbd>                           | Jump to headers
<kbd>F7</kbd>                           | Jump to search
<kbd>F8</kbd>                           | Jump to response headers
<kbd>F9</kbd>                           | Jump to response body

## TODO

* Colors
* Response specific filters (xpath, etc..)
* Better navigation
* File upload
* Autocompletion
* Tests


## Bugs

Bugs or suggestions? Visit the [issue tracker](https://github.com/asciimoo/wuzz/issues)
or join `#wuzz` on freenode
