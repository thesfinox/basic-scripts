# Bookmarksi3

## Description

`bookmarksi3` manages web bookmarks through a dynamic menu and lets the user open web pages in a browser session. It works best in the case of i3 window manager as a dynamic menu to quickly access  frequently browsed pages.

## Prerequisites

* [dmenu](https://tools.suckless.org/dmenu/)
* a web browser \(such as [Firefox](https://www.mozilla.org/en-US/firefox/)\)
* a text editor \(such as [Vim](https://www.vim.org/)\)

{% hint style="info" %}
`bookmarksi3` first checks whether the environmental variable `$BROWSER` is set and uses the browser to which it points, otherwise it reverts the the default choice of the desktop environment \(using `xdg-open`\).

The same policy applies to the choice of the text editor: it first checks for the definition of `$EDITOR`, then for the default choice of `xdg-open` and eventually to `nano`.
{% endhint %}

{% hint style="info" %}
In principle it is also possible to use other dynamic menus for X such as [rofi](https://github.com/davatorium/rofi), but it greatly exceeds the simple needs of this script. In this case you need to change `dmenu` to `rofi -dmenu` in the script.

The best experience should be delivered when `dmenu` is installed in a vanilla version through a package manager such as [pacman](https://www.archlinux.org/pacman/) or [apt](https://wiki.debian.org/Apt). E.g. `# pacman -S dmenu`.
{% endhint %}

## Usage

You can use `bookmarksi3` in several ways:

* `bookmarksi3 -m`: opens a dynamic menu which allows the user to select the bookmark to open;
* `bookmarksi3 -e`: directly edit the text file where all the bookmarks are stored;
* `bookmarksi3 -u URL -n NAME`: add URL to the text file with NAME as label.

Its recommended usage is to bind `bookmarksi3 -m` to a keyboard shortcut, while other combination should be used in a comman line environment.

{% hint style="danger" %}
Options `-u` and `-n` must be used at the same time in order for the script to work properly.
{% endhint %}

{% hint style="info" %}
The script looks for the text file in the _config_ directory of the current user \(`~/.config/bookmarksi3/bookmarks.list` by default\). If the directory has been moved by `xdg-user-dir` then the scripts automatically looks for the path. As a last resource, it automatically creates the file in the default location.
{% endhint %}

{% hint style="info" %}
You can use `bookmarksi3 -h` to display usage and help.
{% endhint %}

