CR2 - `ufraw` и `raw-thumbnailer`
HEIC - `libheif-tools`

```shell
sudo dnf install -y libheif-tools ufraw

sudo nano /usr/share/thumbnailers/gdk-pixbuf-thumbnailer.thumbnailer
```

В `MimeType=` добавить `image/x-xpixmap;image/x-canon-cr2;`

```shell
rm -rf .cache/thumbnails/* .thumbnails/*
```