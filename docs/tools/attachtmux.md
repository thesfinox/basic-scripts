# Attachtmux

## Description

`attachtmux` can be used to attach the terminal multiplexer [tmux](https://github.com/tmux/tmux/wiki) to a previous active session of the terminal.

## Prerequisites

* [tmux](https://github.com/tmux/tmux)
* [dmenu](https://tools.suckless.org/dmenu/)

{% hint style="info" %}
In principle you could also use other dynamic menus for X, such as [rofi](https://github.com/davatorium/rofi) \(in this case you just need to change `dmenu` with `rofi -dmenu` in the source code\). This alternative is also more customisable, but greatly exceeds the simple needs of the script.
{% endhint %}

{% hint style="warning" %}
Technically you can customise [dmenu](https://tools.suckless.org/dmenu/) while compiling it or with [patches](https://tools.suckless.org/dmenu/patches/). This script was however written for a vanilla copy of the software and might not work with a patched version \(the best option would be to install it through a package manager such as [pacman](https://www.archlinux.org/pacman/) or [apt](https://wiki.debian.org/Apt). E.g.: `# pacman -S dmenu`\).
{% endhint %}

## Usage

The script displays a dropdown menu from which you can choose the active session to reattach.

Simply bind a keyboard shortcut to `attachtmux` and select the session from the menu.

{% hint style="info" %}
Input `attachtmux -h` in the terminal to display usage and help.
{% endhint %}

