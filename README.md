# Dev environment setup

This is my personal environment setup for **Arch Linux**, btw.
Using Wayland with Hyprland and **NeoVim** ofc.


<p align="center">
<img src="images/handshake.png" alt="arch-neovim-handshake" style="height=300">
</p>

## Usage

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

### Credit
Based on ThePrimeagen's [dev](https://github.com/ThePrimeagen/dev)
