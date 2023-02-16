# Dotfiles
Configuration for Debian Bookworm with i3wm, Polybar and Rofi. It also includes configuration for alacritty, dunst, picom, and zathura.

Inspired by Keyitdev/dotfiles, including Catppuccin themes.

## Usage
## Install dependencies
```bash
sudo apt update
sudo apt install acpi alsa-utils curl pulseaudio xorg alacritty btop dunst feh firefox i3 libnotify light mpc mpd ncmpcpp nemo neofetch neovim papirus-icon-theme picom polybar ranger rofi scrot slop xclip zathura fontconfig
```

## Install i3lock-color
i3Lock-color isn't currently on the debian repos. To install, follow the instructions from original repo

```
sudo apt install autoconf gcc make pkg-config libpam0g-dev libcairo2-dev libfontconfig1-dev libxcb-composite0-dev libev-dev libx11-xcb-dev libxcb-xkb-dev libxcb-xinerama0-dev libxcb-randr0-dev libxcb-image0-dev libxcb-util0-dev libxcb-xrm-dev libxkbcommon-dev libxkbcommon-x11-dev libjpeg-dev
git clone https://github.com/Raymo111/i3lock-color.git
cd i3lock-color
./install-i3lock-color.sh
```

## Clone and install this repo
```
git clone git@github.com:alimaldonado/dotfiles.git
cd dotfiles
```

- Fonts
```
sudo cp -r ./fonts/* /usr/share/fonts
# user install
# cp fonts/* ~/.fonts/
fc-cache -v -f
```
- Scripts
```
sudo cp -r ./scripts/* /usr/local/bin
```

- Config

```bash
cp config/* ~/.config/
# install catpuccin for rofi. Follow original repo instructions
cd ~/.config/rofi/catppuccin/basic/
bash install.sh
```

