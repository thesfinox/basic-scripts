# Battery

## Description

`battery` displays information on the current state of the battery of the laptop.

## Prerequisites

* [acpi](http://www.acpi.info/)

{% hint style="info" %}
Depending on your kernel configuration different modules can be available. The modules in the script should however be available in almost all cases.
{% endhint %}

## Usage

Simply input `battery` in the terminal to display information on the battery and its charge. The script will display in order:

* **percentage** of the charge \(e.g.: 50%, 60%, etc.\)
* current **status**:
  * arrow pointing upwards = charging
  * arrow pointing downwards = discharging
  * power plug = maximum charge reached and currently plugged-in
* **graphic** information on the battery:
  * warning sign = must connect to power plug
  * filling battery = not fully charged
  * smiling face = battery is fully charged

{% hint style="info" %}
Input `battery -h` in the terminal to display usage and help.
{% endhint %}

