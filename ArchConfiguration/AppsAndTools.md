# configure  pacman's mirror image

```bash
sudo pacman -S reflector
```

Backup the mirror image list:

```bash
sudo cp /etc/pacman.d/mirrorlist /etc/pacman.d/mirrorlist.bak
```

Update the mirror list depending on the speed:

```bash
sudo reflector --verbose --latest 10 --protocol https --sort rate --save /etc/pacman.d/mirrorlist
```

## Neovim

Install Neovim to edit the configs

We using the init.lua file, make a nvim direcroty in ~/.config/ and create a init.lua file,
then copy paste the init.lua in my repo -dotfiles-.

## Some useful apps & tools

```bash
sudo pacman -S p7zip zip unzip unrar htop wget locate fzf man-db ripgrep
yay -S timeshift gnome-shell-pomodoro speedtest-cli
```

Run this command once

```bash
sudo updatedb
```

## Zoxide -cd alternative-
```bash
sudo pacman -S zoxide
```

watch Dreams of code vid to configure it <https://www.youtube.com/watch?v=aghxkpyRVDY>

## Fonts

```bash
sudo pacman -S ttf-jetbrains-mono-nerd
```

## install java

```bash
sudo pacman -S jdk-openjdk
```

## install basic apps

```bash
sudo pacman -S libreoffice-fresh vlc gimp krita inkscape obs-studio
```

## install tmux

```bash
sudo pacman -S tmux
```

Copy my tmux.conf into the tmux folder & clone TPM

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
Then install them with prefix + I

## Zathura

A light wieght pdf reader

Will not work with pdf by default, you ,might need to install this:

```bash
sudo pacman -S zathura zathura-pdf-mupdf
```

Read more on <https://wiki.archlinux.org/title/Zathura>

 *Tips and tricks

Commands may be entered directly into zathura by pressing :, just like in vi.
Enable copy to clipboard

`~/.config/zathura/zathurarc`

`set selection-clipboard clipboard`

* Side-by-side mode

Press d to toggle side-by-side mode.

In side-by-side mode, to view odd pages on the left side, enter the command
set first-page-column 1:1 into zathura. This is particularly useful for reading
two-page illustrations or music scans where typesetting optimizes page-turning
on certain pages.

`~/.config/zathura/zathurarc`

```config
map D set "first-page-column 1:1"
map <C-d> set "first-page-column 1:2"
```

Or install alternative:

## llpp

```bash
yay -S llpp
```
## Obsidian

## Installation

* using pacman:

```bash
sudo pacman -S obsidian
```

* Using flatpak:

```bash
flatpak install flathub md.obsidian.Obsidian
```
