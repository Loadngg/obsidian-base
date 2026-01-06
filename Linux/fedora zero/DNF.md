В терминале выполняем:

```bash
sudo gnome-text-editor /etc/dnf/dnf.conf
```

и добавляем в конец файла следующие параметры:

```
fastestmirror=True
max_parallel_downloads=10
defaultyes=True
keepcache=True
```

Далее выполняем:

```bash
sudo dnf autoremove && sudo dnf clean all
```

#dnf