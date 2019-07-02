# Attachtmux

## Description

`attachtmux` can be used to attach to a previous active session of the terminal multiplexer [tmux](https://en.wikipedia.org/wiki/Tmux). In order to use the script you should have both [tmux](https://en.wikipedia.org/wiki/Tmux) and [dmenu](https://tools.suckless.org/dmenu/) installed, as the tool uses the latter to display and select active sessions.

## Prerequisites

* `tmux` \([link](https://en.wikipedia.org/wiki/Tmux)\) 
* `dmenu` \([link](https://tools.suckless.org/dmenu/)\)

{% hint style="info" %}
In principle you can also use other dynamic menus for X, such as [rofi](https://github.com/davatorium/rofi). Its implementation is pretty straightforward: changing `dmenu` to `rofi -dmenu` in the script should be enough. This alternative is also more customisable and versatile, but exceeds the actual needs of the script.
{% endhint %}

{% hint style="warning" %}
You can customise [dmenu](https://tools.suckless.org/dmenu/) during compilation and patch it to fulfil your needs. This script was written for a vanilla copy of the tool \(best if installed through a package manager, such as [pacman](https://www.archlinux.org/pacman/). E.g.: `# pacman -S dmenu`\).
{% endhint %}

## Usage

Simply bind a keyboard shortcut to `attachtmux` and select the session you want to restore.

{% hint style="info" %}
Use `attachtmux -h` in the terminal to show usage and help.
{% endhint %}

