# st - simple terminal

st is a simple terminal emulator for X which sucks less.

## Patches

* [scrollback](https://st.suckless.org/patches/scrollback/st-scrollback-20210507-4536f46.diff)
* [ligatures](https://st.suckless.org/patches/ligatures/0.8.4/st-ligatures-boxdraw-20210824-0.8.4.diff)
* [bold-is-not-bright](https://st.suckless.org/patches/bold-is-not-bright/st-bold-is-not-bright-20190127-3be4cf1.diff)
* [clipboard](https://st.suckless.org/patches/clipboard/st-clipboard-0.8.3.diff)
* [delkey](https://st.suckless.org/patches/delkey/st-delkey-20201112-4ef0cbd.diff)
* [xresources-signal-reloading](https://st.suckless.org/patches/xresources-with-reload-signal/st-xresources-signal-reloading-20220407-ef05519.diff)
* [anysize](https://st.suckless.org/patches/anysize/st-anysize-0.8.4.diff)
* [font2](https://raw.githubusercontent.com/oncomouse/patches/master/st-font2-20210629-4ef0cbd.diff)
* [undercurl](https://raw.githubusercontent.com/oncomouse/patches/master/st-undercurl-20220322-ef05519.diff)
* [desktopentry](https://st.suckless.org/patches/desktopentry/st-desktopentry-0.8.4.diff)
* [boxdraw](https://raw.githubusercontent.com/oncomouse/patches/master/st-boxdraw-20220323-ef05519.diff)

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```
tic -sx st.info
```

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
