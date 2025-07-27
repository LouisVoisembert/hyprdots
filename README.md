# 💜 Hyprdots

My personal dotfiles for a minimal, violet-themed **Wayland** setup based on [Hyprland](https://github.com/hyprwm/Hyprland), using `waybar`, `wofi`, `alacritty`, and more.  
All configs are modular and managed with [GNU Stow](https://www.gnu.org/software/stow/).

> ⚠️ Work in progress – feel free to fork or watch!

---

## 🧰 Components

| Module      | Description                            |
|-------------|----------------------------------------|
| `hypr`      | Hyprland WM config                     |
| `waybar`    | Custom bar with network, volume, etc.  |
| `wofi`      | App launcher styled in violet          |
| `alacritty` | Terminal configuration                 |
| `wlogout`   | Logout menu with themed icons          |
| `neofetch`  | Terminal system info                   |
| `zsh`       | Shell setup with aliases + prompt      |
| `wallpaper` | Personal wallpapers (hyprpaper)        |

---

## 📸 Screenshots


<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/9bcbbbef-9351-42f7-8385-7ecfb93e2454" />

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/0998d974-1e21-46f0-9316-7e28aca66068" />


---

## 📦 Install

Before installing, make sure to **backup any existing config files** you don't want to overwrite.

If you encounter a `stow` conflict like:

```bash
WARNING! stowing X would cause conflicts:

    existing target is not owned by stow: ...
```

It means a file or folder already exists. You need to **remove it or move it manually**:

```bash
rm -rf ~/.config/waybar
```
```bash
git clone git@github.com:LouisVoisembert/hyprdots.git ~/.dotfiles
cd ~/.dotfiles
stow hypr waybar wofi alacritty zsh
```

## ❌ Uninstall

To remove a specific module, use:

```bash
stow -D waybar
```

