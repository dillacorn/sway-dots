# `dilla.sway`
distro: [`debian sid`](https://www.debian.org/releases/sid/) | Wayland: [`sway-wm`](https://github.com/swaywm/sway) | kernal: [`linux-tkg`](https://github.com/Frogging-Family/linux-tkg) - [`install linux-tkg on debian`](https://github.com/Frogging-Family/linux-tkg?tab=readme-ov-file#deb-debian-ubuntu-and-derivatives-and-rpm-fedora-suse-and-derivatives-based-distributions)

### `~click picture!~`
[![preview](https://i.imgur.com/1JOMnpC.png)](https://youtu.be/sL1O7zuQIuE)

# my keybinds are **DWM** inspired

My keybinds (see [**sway**](https://github.com/dillacorn/sway-dots/blob/main/config/sway/config) are [**suckless DWM**](https://dwm.suckless.org/) inspired.

Previously used [**DWM Flexipatch**](https://github.com/bakkeby/dwm-flexipatch) by [bakkeby](https://github.com/bakkeby) ~ DWM was my very first window manager.

# wallpapers

[gruvbox](https://github.com/AngelJumbo/gruvbox-wallpapers) by [AngelJumbo](https://github.com/AngelJumbo)

[aesthetic-wallpapers](https://github.com/D3Ext/aesthetic-wallpapers) by [D3Ext](https://github.com/D3Ext)

# keybind commands/navigation

READ [sway](https://github.com/dillacorn/sway-dots/blob/main/config/sway/config) config for keybinds + alternative [sway](https://github.com/dillacorn/sway-dots/blob/main/config/sway/super_navigation.config) config for mod4(win/super) navigation keybinds

Using both `mod1(alt)` and `mod4(win/super)` in default config depending on use.

`mod4+shift+q` = reloads config

`mod4+shift+r` = rotates sway/i3 navigation configurations -> [see sway dir.](https://github.com/Dillacorn/sway-dots/tree/main/config/sway)

`mod4+shift+g` = capture a gif with script <- `repeat keybind to finish command!`

`mod4+shift+s` = grimshot screenshot

`mod4+ctrl+shift+s` = flameshot screenshot

# terminal navigation

`ctrl+l` <- clears console

`ctrl+a` <- goes to beginning of line

`ctrl+e` <- goes to end of line

`ctrl+k` <- deletes from cursor to end of line

`ctrl+left` or `ctrl+right` <- forward and backward words

`shift+PgUp` or `shift+PgDwn` <- up and down terminal (faster than scrolling)

more commands to learn -> [learning-command-line](https://github.com/LinkedInLearning/learning-linux-command-line-3005201/blob/e0cfdc8244b804b57c04b5cffc55c0b322122457/commands.md) by [LinkedInLearning](https://github.com/LinkedInLearning)

# run a script in [scripts folder](https://github.com/dillacorn/sway-dots/tree/main/scripts)

example:

### NOTE: run these commands individually

```sh
cd ~/dotfiles/scripts
chmod +x install_my_apps.sh
sudo ./install_my_apps.sh
```

# drop the display managers...full stop...

I've had the most issues with display (login) managers, so I prefer TTY. To remove your display manager, use:

```sh
sudo apt remove gdm3 sddm lightdm
```

Login by typing your username and password, then start Sway from TTY by typing:

### **sway**
```sh
sway
```

If you encounter issues, switch TTYs with CTRL+ALT+F1 to F6.

### I've discovered!
**HUGE PRO** to using the **TTY** is if you have `Sway` config issues or an application is experiencing errors when you logout of `Sway` you will see those errors in the **TTY!**

# prefer X11 over Wayland? Have an Nvidia GPU?

Use [**i3 wm**](https://github.com/i3/i3) instead till **Nvidia** is fully supported... or if you just like **X11** over **Wayland** due to strange behavior and/or bugs with your specific hardware.

# See my [i3 wm repo](https://github.com/dillacorn/dotfiles)
# I personally use i3 over Sway... Mostly due to prefrence and lack of customizability wlroots locks down on its users

# converting sway config to i3?

```sh
i3 -C -c ~/.config/i3/config
```
