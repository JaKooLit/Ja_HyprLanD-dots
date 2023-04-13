
https://user-images.githubusercontent.com/85185940/227948968-03e5097d-9850-437f-8109-8d376bf81e9f.mp4


<br>
<h3 align = "center"> Arch / Gentoo Hyprland Dotfiles</h3>
<br>

<img src="https://github.com/JaKooLit/Ja_HyprLanD-dots/blob/main/preview/Arch.png" alt="">

<img src="https://github.com/JaKooLit/Ja_HyprLanD-dots/blob/main/preview/Gentoo.png" alt="">

## Components:

- Main Component:[`Hyprland`](https://github.com/hyprwm/Hyprland)
- Terminal: [`Foot`](https://github.com/r-c-f/foot)
- Shell: [`Zshell`](https://www.zsh.org/)
- Status bar: [`Waybar`](https://github.com/Alexays/Waybar)
- Menu : [`Wofi`](https://hg.sr.ht/~scoopta/wofi)
- FIle Manager: [`Thunar`](https://docs.xfce.org/xfce/thunar/start)

## Miscellaneous:

- Themes: `Dracula`
- Cursor theme: `Bibata Modern Ice`

## Needed packages:

(all of the above components) plus

`swaybg` - for wallpaper

`swayidle` - not necessary but you can install

`swaylock-effects` - or swaylock

`wlroots` `wlogout` `cava` `polkit-gnome`

`mako` - for notifications

`grim` `slurp` `wl-clipboard` - for screenshot

`brightnessctl`  - for monitor and keyboard brightness - not needed for desktop

`mpv` - for wofi beats to work

`viewnior` or `swayimg`  

`pamixer` - for volume control notification. 

`playerctl` - keyboard hotkeys multimedia controls

`xorg-xwayland` - needed to run some non-wayland app especially games

`fonts` - required awesome fonts. AUR and official repo have... else most of the waybar modules wont work. Most of configs here I used Fantasque Sans Mono. I used Cascadia Code Semibold Italic on foot.

`pipewire` - needed pipewire pipewire-pulse pipewire-alsa



## ✨ Arch Linux quick Installation:

A guide to install :[`Youtube Link`](https://youtu.be/_deaeSU1WK8)

Dual Boot Guide :[`Youtube Link`](https://www.youtube.com/watch?v=ADYqS8psSJ0)

1.) optional: you can install nvidia-all driver from Frogging Family to replace the nvidia-drivers 
 - chmod +x nvidia-all-driver and run with nvidia-all-driver

a.) Install yay (chmod +x yay-bin-install and run the script). You can also install paru if desired

a.1) paru-hyprland was created to use paru instead of yay. Paru will be installed automatically if you select yes during the installation. make sure to run (chmod +x paru-hyprland first and run the script)

b.) You can install one by one packages or choose the automatic installer script. (chmod +x install-hyprland and run the script). 
NOTE. If you install paru instead of yay, ensure to edit install-hyprland and change all yay with paru

c.) If you want to add or edit packages, edit install-hyprland script. Check first if packages are present on AUR or official else the script will fail.

d.) Installation of Asus-ROG-utilities are entirely optional. if you select no, will skip the step.



## ✨ Manual Installation and Notes: 
### you can copy, create, change, however, would appreciate if you have have a better solution / changes so we will all improve :)

These configs are used in my Laptop and Desktop. 
Please note, Only provided are configs. Any Hyprland-related issues to be reported on Hyprland Github

a.) Copy / Move files / folders in your ~/.config

b.) Put wallpapers in your ~/Pictures/

c.) if you want in Arch, make sure to comment / uncomment some items in /hypr/configs/exec.conf - location of polkit is different than gentoo, By default, all configs are set to work with Arch Linux

d.) If you use `thunar` as file manager, suggested additions for thunar (thunar-volman, tumbler, gvfs, gvfs-mtp (for accessing phone), Thunar archive plugin-ins) See Arch wiki https://wiki.archlinux.org/title/thunar

e.) make sure scripts located at /hypr/scripts/ are executable as required. (use chmod +x or right click, properties, change permission to be executable)

f.) Inspect /hypr/configs/exec.conf Choose which polkit gnome to use. to use. (Gentoo have different location of executables. Arch /usr/lib vs Gentoo /usr/libexec) Polkits by default are set to Arch Linux

g.) if you have azerty keyboard [`this`](https://github.com/swaywm/sway/issues/1460?fbclid=IwAR1C8VcY_wWbGhXvT-5ApjJCQuJoJzhOVor6o5fdn0Nj1c6bD9JXoQAPQIg) might help



## ✨ Gentoo Specific notes

<details>
<summary>
Gentoo Specific
</summary>

1. [`Hyprland - Link to zugaina`](https://gpo.zugaina.org/gui-wm/hyprland) have 3 overlays. I am using wayland-desktop overlay. Nvidia and openrc users, you should look into thegreatmcpain overlay. Or of course you can compile hyprland from source
2. Waybar - from Gentoo repo's waybar, I experienced unclickable workspaces. I have installed from useless-overlay. Click [`here`](https://github.com/JaKooLit/Ja_HyprLanD-dots/blob/main/misc/Gentoo-Waybar) for guidance
3. For screen sharing, I use xdg-desktop-portal-wlr which seems to work. If you are having issues, install xdg-desktop-portal-hyprland
4. if you use openrc, ensure to launch hyprland with dbus-run-session Hyprland. Omitting the dbus-run-session may cause [`runtime errors`](https://wiki.gentoo.org/wiki/Sway#Failed_to_connect_to_user_bus)
5. `fonts` you need fontawesome and nerd-fonts use (3270 + symbols) (available in overlay) to display some icons in waybar

