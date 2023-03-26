### Hyprland-dotfiles ###

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

`fonts` - required awesome fonts. AUR and official repo have... else most of the waybar modules wont work. Most of configs here I used Fantasque Sans Mono

## Gentoo Specific:

1. [`hyprland`](https://gpo.zugaina.org/gui-wm/hyprland) have 3 overlays. I am using wayland-desktop overlay. Nvidia and openrc users, you should look into thegreatmcpain overlay. Or of course you can compile hyprland from source
2. Waybar - from Gentoo repo's waybar, I experienced unclickable workspaces. I have installed from useless-overlay. Click [`here`](https://github.com/JaKooLit/Ja_HyprLanD-dots/blob/main/misc/Gentoo-Waybar) for guidance
3. For screen sharing, I use xdg-desktop-portal-wlr which seems to work. If you are having issues, install xdg-desktop-portal-hyprland
4. if you use openrc, ensure to launch hyprland with dbus-run-session Hyprland. Omitting the dbus-run-session may cause [`runtime errors`](https://wiki.gentoo.org/wiki/Sway#Failed_to_connect_to_user_bus)


## Notes: 

These configs are used in my Laptop and Desktop. 

a.) Copy / Move files / folders in your ~.config

b.) Put wallpapers in your ~Pictures/

c.) if you want in Arch, make sure to comment / uncomment some items in /hypr/configs/exec.conf - location of polkit is different than gentoo

d.) If you use `thunar` as file manager, suggested additions for thunar (thunar-volman, tumbler, gvfs, gvfs-mtp (for accessing phone), Thunar archive plugin-ins) See Arch wiki https://wiki.archlinux.org/title/thunar

e.) make sure scripts located at /hypr/scripts/ are executable as required. (use chmod +x or right click, properties, change permission to be executable)

f.) Inspect /hypr/configs/exec.conf Choose xdg-desktop-portal to use. (Gentoo have different location of executables. Arch /usr/lib vs Gentoo /usr/libexec

g.) if you have azerty keyboard [`this`](https://github.com/swaywm/sway/issues/1460?fbclid=IwAR1C8VcY_wWbGhXvT-5ApjJCQuJoJzhOVor6o5fdn0Nj1c6bD9JXoQAPQIg) might help
