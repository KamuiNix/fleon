# Fleon WM
A next-generation X11 window manager built with C and XCB. This project aims to combine features of many of the popular windows managers. For example, you could have i3 tabs with a binary spaced partitioning layout. Or a full fledged floating mode with configurable titlebars which you could toggle into. Wayland support is also planned.

## Building 

You will need the following dependencies first:
1. [`libxcb-1.14`](https://xcb.freedesktop.org/) 

```bash
$ git clone https://github.com/kamui-7/fleon.git
$ cd fleon
$ make
```

## Contributing

Contributions are always welcome. For a development environment, we recommend using [Xephyr](https://www.freedesktop.org/wiki/Software/Xephyr/), which is a nested X server, to test and debug. 

To setup the nested X server, run:
```bash
Xephyr -br -ac -noreset -screen 1500x900 :1
```

Running the window manager inside of Xephyr is just a matter of passing in the right `DISPLAY` variable.
```bash
DISPLAY=:1 ./build/fleon
```

## License
Featherbox is available under the GNU General Public License v3. See the LICENSE file for more info.
