# Clipboard

## Description

`clipboard` use a simple tool to manage both primary and secondary clipboard in X. It can print the content of the clipboard or show it as a system notification. It also produces a QR code to share the content of the clipboard with other devices.

## Prerequisites

* [clipit](https://github.com/CristianHenzel/ClipIt)
* an image viewer \(such as [feh](https://feh.finalrewind.org/), optional\)
* Python [QR code](https://pypi.org/project/qrcode/) library \(optional\)
* notification server \(such as [dunst](https://dunst-project.org), optional\)

{% hint style="info" %}
In principle the script does not require an image viewer to display the QR code as long as the terminal can display the output. For better quality and the possibility to share to other devices, we recommend installing either [feh](https://feh.finalrewind.org/) or [sxiv](https://github.com/muennich/sxiv). E.g.: `# pacman -S feh`.
{% endhint %}

{% hint style="info" %}
The QR code library is not necessary if you do not wish to share the content of the clipboard with other devices. However we recommend installing it for its simplicity in the exchange of information among PC, phone, tablet, etc. E.g.: `# pacman -S python-qrencode`.
{% endhint %}

{% hint style="info" %}
The notification server is not required for the script to work, but it is highly recommended to show the content of the clipboard outside a terminal environment.
{% endhint %}

## Usage

It is possible to use the script in many different ways. For example, let `BUF` be a choice between `primary` or `clipboard` to differentiate between the primary selection \(higlighted content\) and clipboard \(CTRL+C\), then:

* `clipboard -c BUF`: print the content of the clipboard `BUF` to the standard output;
* `clipboard -n BUF`: show the content of the clipboard `BUF` as a system notification;
* `clipboard -q BUF`: show the content of the clipboard `BUF` as QR code.

{% hint style="info" %}
You can use `clipboard -h` to display usage and help.
{% endhint %}

