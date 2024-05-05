### Включаем Non-free репозиторий:

```bash
sudo dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

### Устанавливаем зависимости:

```bash
sudo dnf update && sudo dnf upgrade --refresh && sudo dnf install curl gamemode icoutils libcurl wget zenity bubblewrap zstd cabextract tar goverlay openssl --skip-broken
```

### Стандартная установка:

```bash
wget -c "https://github.com/Castro-Fidel/PortWINE/raw/master/portwine_install_script/PortProton_1.0" && sh PortProton_1.0
```

> [!info] Все ярлыки создаются в папке ~/.local/share/applications

>[!bug] При ошибке открытия через ярлык нужно отредактировать `PortProton.desktop`, убрав кавычки в путях к папке

#portproton #proton