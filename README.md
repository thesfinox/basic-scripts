# Tools and Scripts

## Table of Contents

* [Introduction](./#introduction)
* [Description of the Tools](./#description-of-the-tools)
  * [attachtm](./#attachtmux-link)[ux](./#prerequisites)
    * [Prerequisites](./#prerequisites)
    * [Usage](./#usage)

## Introduction

This tools are simple implementation of basic tasks we personally use in our desktop setup. They span across several applications, from using the terminal in a productive way to mounting hard drives and Android phones, etc.

The scripts are based on personal experience and may not provide a good user experience to everybody, but they will at least cover the basics for everyone.

## Description of the Tools

### Attachtmux \([link](https://raw.githubusercontent.com/thesfinox/basic-scripts/master/scripts/attachtmux)\)

`attachtmux` can be used to attach to a previous active session of the terminal multiplexer [tmux](https://en.wikipedia.org/wiki/Tmux). In order to use the script you should have both [tmux](https://en.wikipedia.org/wiki/Tmux) and [dmenu](https://tools.suckless.org/dmenu/) installed, as the tool uses the latter to display and select active sessions.

#### Prerequisites

* `tmux` \([link](https://en.wikipedia.org/wiki/Tmux)\) 
* `dmenu` \([link](https://tools.suckless.org/dmenu/)\)

In principle you can also use other dynamic menus for X, such as [rofi](https://github.com/davatorium/rofi). Its implementation is pretty straightforward: changing `dmenu` to `rofi -dmenu` in the script should be enough. This alternative is also more customizable and versatile, but exceeds the actual needs of the script.

#### Usage

Simply bind a keyboard shortcut to `attachtmux`. 

Use `attachtmux -h` in the terminal to show usage and help.

## License

This work is licensed under the MIT License, thus «THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.»

