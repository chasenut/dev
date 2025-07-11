# Dev environment setup

This is my personal environment setup for **Arch Linux** (btw).
Using Wayland with Hyprland and **NeoVim**.


<p align="center">
<img src="images/handshake.png" alt="arch-neovim-handshake" style="height=200">
</p>

# Usage

This repo should be located as such: `$HOME/personal/dev`.
```
mkdir -p ~/personal
cd ~/personal
```

Download this repo over to `~/personal/dev`.

To run the main scripts located in the root directory of this repo, prefix them with assigning `$DEV_ENV` system variable.
This can be done with this command **while in the root of this repository** (`~/personal/dev`):
```
DEV_ENV=$(pwd) ./<script>
```
*Replace <script> with `dev-env`, `run`, or `init`.*
You can also run `dev-env` and `run` with a `--dry` flag at the end of the command to see what's going to happen.

### Sound
You can use `pavucontrol` for sound management. I'm also using script `audiofix` located in
`env/.local/scripts/audiofix` (in this repo).
It is being run from the bottom of `.zsh_profile` which you can find in `env/`.

### Wallpapers
This setup is using `swaybg` (**hyprpaper** is very buggy) for handling wallpapers. 
By default (check `env/.config/hypr/hyprland.conf`) it loads `~/personal/wallpapers/default.jpg`
so make shure you have that one, **wallpaper files are not included in this setup**. 
You can also switch wallpapers very easily using `setbg` command, 
which is located in `env/.local/scripts/setbg`.
It opens a `fzf` menu where you can select wallpaper from `$HOME/personal/wallpapers/` directory.

> [!IMPORTANT]
> This setup looks for wallpapers in `~/personal/wallpapers/` directory, which does not come included.
> You need to create it yourself or change the configs.

### Greeter SDDM
If you are using SDDM as your greeter, you may also want to make it nice looking.
I can recommend [sddm-astronaut-theme](https://github.com/Keyitdev/sddm-astronaut-theme).
*With bigger display resolution you may need to tinker a little bit with font size in cofing*

---

### Credit
Inspired by ThePrimeagen's [dev](https://github.com/ThePrimeagen/dev)
