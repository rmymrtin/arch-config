## Preview
![Preview](/preview.png)

## Theme
https://gitlab.com/kalilinux/packages/kali-themes

## Softwares
- git
- firefox
- google-chrome
- postman-bin
- spotify
- visual-studio-code-bin
- libreoffice-still
- xfce4-multiload-ng-plugin

## Updated configs (settings paths for xfce)
* Settings Manager
    * Appearance
        * Style: Kali-Dark
        * Icon: Flat-Remix-Blue-Dark
        * Font
            * Default Font: Sans Regular 10pt
            * Default Monospace Font: Monospace Regular 10pt
* Terminal
    * Appearance
        * Font
            * Use system font (no)
            * Source Code Pro Regular 10pt
    * Colors
        * Presets
            * Kali
* Panel preferences
    * Panel 1
        * Items
            * Applications Menu
                * Button title: ' Applications' (add space before)
                * Icon: kali-menu
            * Add multiload-ng plugin (select Processor, Memory, Network, Swap)

## Commands

### Install AUR helper
```bash
pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si
```

### Install softwares
```bash
yay -S git firefox google-chrome postman-bin potify visual-studio-code-bin libreoffice-still xfce4-multiload-ng-plugin
```

### Install themes & icons
```bash
sudo cd ~ && git clone https://gitlab.com/kalilinux/packages/kali-themes && mkdir -p ~/.local/share/themes; mv ~/kali-themes/share/themes/* ~/.local/share/themes && mkdir ~/.icons && cd -R ~/kali-themes/share/icons/* ~/.icons && cp ~/kali-themes/share/color-schemes/* /usr/share/xfce4/terminal/colorschemes/
```
