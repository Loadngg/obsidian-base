### Включаем Non-free репозиторий:

```
sudo dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

### Устанавливаем зависимости:

```
sudo dnf update && sudo dnf upgrade --refresh && sudo dnf install curl gamemode icoutils libcurl wget zenity bubblewrap zstd cabextract tar goverlay openssl --skip-broken
```

### Стандартная установка:

```
wget -c "https://github.com/Castro-Fidel/PortWINE/raw/master/portwine_install_script/PortProton_1.0" && sh PortProton_1.0
```

> [!info] Все ярлыки создаются в папке ~/.local/share/applications

#portproton #proton