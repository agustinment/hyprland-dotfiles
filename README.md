# Hyprland Dotfiles

Mi configuración de Hyprland con Waybar, swaybg y teclas en español (latam)

## Instalación

```bash
# Clonar como bare repo
git clone --bare https://github.com/agustinment/hyprland-dotfiles.git $HOME/.dotfiles

# Configurar alias
alias dotfiles='git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
dotfiles checkout

# Permisos
dotfiles config --local status.showUntrackedFiles no
hyprctl reload
```

## Dependencias (Arch)
```bash
sudo pacman -S hyprland waybar swaybg wofi kitty
```

## Estructura
.config/
├── hypr/ # hyprland.conf + keybinds
├── waybar/ # config + style.css
└── kitty/
