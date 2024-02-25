# Read this <https://github.com/prasanthrangan/hyprdots/wiki/FAQ>

## Monitor settings

```bash
nvim ~/.config/hypr/monitors.conf
```

The general config of a monitor looks like this

monitor=name,resolution,position,scale

A common example:

monitor=eDP-1,1920x1080@60,0x0,1

will tell Hyprland to make the monitor on DP-1
a 1920x1080 display, at 144Hz, 0x0 off from the top left corner,
with a scale of 1 (unscaled).

To list all available monitors (active and inactive):

hyprctl monitors all

See <https://wiki.hyprland.org/Configuring/Monitors/>

## Hyprland settings

Costume settings in ~/.config/hypr/userprefs.conf

```bash
nvim ~/.config/hypr/userprefs.conf
```
then add your costume config or copy mine.

## emoji and symbols

<https://wiki.archlinux.org/title/Fonts#Emoji_and_symbols>
