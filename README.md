# Dmenu Scripts

Scripts I use every day.

## Dependencies

On Arch-based systems:

```
alsa
arch-wiki-docs
brave browser
docker
imv
jq
maim
mpc
mpd
mpv
pulseaudio
qutebrowser
reddio
slock
systemd
tee
tmux
udisks2
xargs
xclip
xrandr
xwallpaper or swaybg
yad
youtube-dl
```

## Clone

```bash
git clone https://github.com/adelgado0723/dmscripts
cd dmscripts
```

## Configure

Edit dmscripts/config/config with your preferences. For example:

```
...
DMENU="dmenu -l 20 -p"
DMBROWSER="brave"
DMTERM="alacritty -e"
DMEDITOR="${DMTERM} nvim"
logout_locker='slock'
...
```

## Build and Install

```
sudo make clean build install
```

## Descriptions

### dm-bookman

Search your qutebrowswer bookmarks and quickmarks.

- qutebrowser

### dm-colpick

Copy a color to your clipboard using dmenu, change the colors if needed

- xclip

### dm-confedit

Choose from a list of configuration files to edit.

- none

### dm-currencies

Convert prices between currencies using https://rate.sx

- xclip
- curl

### dm-docker-kill -- needs man entry

Search for a running docker container to kill.

- docker

### dm-docker-rm -- needs man entry

Search for a docker container and remove it.

- docker

### dm-emoji

Select emoji and copy it to clipboard.

- xclip
- python3
- awk
- notify-send

### dm-hub

A hub that you can execute all the other scripts from.

- all other dmscripts dependencies

### dm-icons

Select icon and copy it to the clipboard.

- xclip
- python3
- awk
- notify-send
- curl
- xdotool

### dm-ip

Get IP from interface (or external).

- dig
- ip
- jq

### dm-kill

Search for a process to kill.

- none

### dm-logout

Logout, shutdown, reboot or lock screen.

- systemd
- slock
- notify-send

### dm-maim

Choose type of screenshot to take with maim.

- maim
- tee
- xdotool
- xclip
- xrandr

### dm-man

Search for a manpage or get a random one.

- xargs

### dm-music

Music player using dmenu

- mpd
- mpc

### dm-note

Store multiple one-line texts or codes and copy one of them when needed.

- xclip
- notify-send

### dm-radio

Choose between online radio stations with dmenu.

- mpv
- notify-send
  youtube-dl

### dm-record

Dmenu script to record video,audio,webcam.

- ffmpeg
- pulseaudio
- alsa
- slop (for recording a specific area)

### dm-reddit

Dmenu as a reddit viewer using reddio.

- reddio
- yad

### dm-setbg

A wallpaper setting utility using dmenu, imv and swaybg/xwallpaper

- xwallpaper or swaybg
- imv

### dm-sounds

Choose a ambient background sound to play

- ffmpeg

### dm-tmux-cht.sh -- needs man entry

- tmux
- curl

### dm-tmux-sessionizer -- needs man entry

- tmux

### dm-translate

Translate using Google Translate (through Lingva Translate)

- curl
- jq

### dm-usbmount

Mount or unnmount usb drives using dmenu.

- udisks2

### dm-weather

Simple graphical weather app

- curl
- yad

### dm-websearch

- jq
- brave

### dm-wifi

Connect to wifi using dmenu

- nmcli
- notify-send
- Any Nerd Font

### dm-wiki

Search an offline copy of the Arch Wiki.

- arch-wiki-docs

### dm-youtube

Youtube subscription manager without API access

- curl
- a browser (brave by default)
