Открываем `fstab`

```bash
sudo gnome-text-editor /etc/fstab
```

и добавляем данные параметры после **`compress=zstd:1`** для `/` и `/home`

```
,defaults,noatime,discard=async
```

#fstab
