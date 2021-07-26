# Fullscreen suckless DWM

This is a fork of [suckless dwm](https://dwm.suckless.org) configured for a full screen experience.
It inherits a couple of keybindings from [i3](https://i3wm.org/).

By default, the terminal invoked is [Alacritty](https://github.com/alacritty/alacritty).

### Changed keybindings
- The modkey is now Super (also known as the Windows key), so use it where you would normally use Alt.
- To launch (dmenu)[https://tools.suckless.org/dmenu/], press Super+D.
- To launch the terminal, press Super+Enter.
- The keybinding to show the dwm bar has been removed.

Every other keybinding is the same, albeit the different modkey.

### Standard README
```
dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
```
