# Hyprland-dotfiles

<br>
<h3 align = "center">Gentoo / Arch Hyprland Dotfiles</h3>
<br>

<img src="https://github.com/JaKooLit/Asus-G15-2021-hyprland-dots/blob/main/preview.png" alt="">

<img src="https://github.com/JaKooLit/ASUS_G15-2021_hyprland-dots/blob/main/Gentoo.png" alt="">

## Components:

- Main Component:[`hyprland`](https://github.com/hyprwm/Hyprland)
- Terminal: [`Foot`](https://github.com/r-c-f/foot)
- Shell: [`Zshell`](https://www.zsh.org/)
- Status bar: [`Waybar`](https://github.com/Alexays/Waybar)
- Menu : [`Wofi`](https://hg.sr.ht/~scoopta/wofi)
- FIle Manager: [`Thunar`](https://docs.xfce.org/xfce/thunar/start)

## Miscellaneous:

- Icon fonts: `Shiny Dark Icons`
- Cursor theme: `Bibata Modern Ice`

## Needed packages:

(all of the above components) plus

`swaybg` - for wallpaper

`swayidle` - not necessary but you can install

`swaylock-effects` - or swaylock

`wlroots`  

`mako` - for notifications

`grim` `slurp` `wl-clipboard` - for screenshot

`brightnessctl`  - for monitor and keyboard brightness - not needed for desktop

`mpv` - for wofi beats to work

`viewnior` or sway-img if you prefer  

`polkit-gnome` 

`wlogout` 

`pamixer` - for volume control notification. 

`xorg-xwayland` - needed to run some non-wayland app

## Notes: 

These configs are used in my Laptop and Desktop. 

a.) Copy / Move files / folders in your ~.config

b.) Put wallpapers in your ~Pictures/

c.) if you want in Arch, make sure to comment / uncomment some items in /hypr/configs/exec.conf - location of polkit is different than gentoo

d.) Gento waybar needed different package. Official repo waybar have unclickable workspaces

e.) If you use thunar as file manager, suggested additions for thunar (thunar-volman, gvfs, gvfs-mtp (for accessing phone). Thunar archive plugin-ins) See Arch wiki. These includes thumbnails. Only if desired. https://wiki.archlinux.org/title/thunar

f.) make sure scripts located at /hypr/scripts/ are executable as required. (use chmod +x or right click, properties, change permission to be executable)

g.) Inspect /hypr/configs/exec.conf Choose xdg-desktop-portal to use. (Gentoo have different location of executables. Arch /usr/lib vs Gentoo /usr/libexec
