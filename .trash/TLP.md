## Установка

Устанавливаем `tlp`:
```bash
sudo dnf install tlp tlp-rdw
```

Удаляем прошлый демон:
```bash
sudo dnf remove power-profiles-daemon
```

## Действия после установки

Включаем сервис:
```bash
sudo systemctl enable tlp.service
```

Маскируем службы во избежании конфликтов сервисов:
```bash
systemctl mask systemd-rfkill.service systemd-rfkill.socket
```

Включаем `tlp`:
```bash
sudo tlp start
```

#tlp