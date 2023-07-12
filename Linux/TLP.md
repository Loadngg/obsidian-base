## Установка

Устанавливаем `tlp`:
```
sudo dnf install tlp tlp-rdw
```

Удаляем прошлый демон:
```
sudo dnf remove power-profiles-daemon
```

## Действия после установки

Включаем сервис:
```
sudo systemctl enable tlp.service
```

Маскируем службы во избежании конфликтов сервисов:
```
systemctl mask systemd-rfkill.service systemd-rfkill.socket
```

Включаем `tlp`:
```
sudo tlp start
```

#tlp