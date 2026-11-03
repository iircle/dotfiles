My CachyOS Linux dotfiles.
This currently changes:
- Niri
- iNiR : Keybinds and Styles
- Zsh
- Kitty
- dconf : Nautilus default terminal and keybinds

Required:

```sh
yay -S nautilus-open-any-terminal
dconf load / < ~/.local/share/chezmoi/dconf-settings.ini
```


To dump dconf to a file:
```sh
chezmoi cd
dconf dump / > dconf-settings.ini
```
and remove unsafe things : [org/blueman/plugins/recentconns]
