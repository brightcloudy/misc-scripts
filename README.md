# misc-scripts
## Installation / Usage
  - So far, I only have one thing in here, and I wrote a small Makefile by hand to install it to `$PREFIX`, defaulting to `/usr/local/bin/`. So all that is really necessary to do is the usual:
  ```bash
  make
  sudo make install
  ```
  - Hopefully I'll keep up with this or document if I change my mind about how I want it to work.
## Script Descriptions
### kbd-change
  - `kbd-change` is a script which allows turning off and on the keyboard, touchpad, and trackpoint on my T495 laptop.
  - It can't be executed directly yet, but it has symlinks to provide two commands, `kbd-disable` and `kbd-enable` which do what you'd expect.

## things on the list to go in here:
----
### files
#### sunrise
  - `~/capscontrol.sh`
  - `/usr/share/fonts/Inconsolata-Regular.ttf`
  - `~/.bashrc`
  - `~/.config/i3/net-speed.sh`
  - `/usr/local/bin/tap(toggle|on|off)`
  - `~/uploadclip.sh`
#### prism
  - `/etc/sysctl.conf`
#### skyglow
  - `~/.xdobash`

### programs
  - nitrogen
  - nm-applet
  - xclip
  - vim-X11
  - dunst
  - passmenu
