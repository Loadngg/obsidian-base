```bash
sudo dnf install gcc kernel-headers kernel-devel akmod-nvidia xorg-x11-drv-nvidia xorg-x11-drv-nvidia-libs xorg-x11-drv-nvidia-power nvidia-settings 
```

#### NVidia Optimus
Подключим репозитории RPM Fusion:

```bash
sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

Установим стандартный драйвер NVIDIA для современных видеокарт:

```bash
sudo dnf install gcc kernel-headers kernel-devel akmod-nvidia xorg-x11-drv-nvidia xorg-x11-drv-nvidia-libs
```
```bash
sudo dnf install xorg-x11-drv-nvidia-libs.i686
```

### **Действия по окончании установки:**

По окончании установки необходимо убедиться, что модули ядра были успешно собраны и установлены корректно:

```bash
sudo akmods --force
```

Если возникла ошибка, то подробный журнал можно найти в каталоге `/var/cache/akmods/nvidia/`

Теперь вырежем из образа [initrd](https://ru.wikipedia.org/wiki/Initrd) драйвер nouveau и добавим NVIDIA:

```bash
sudo dracut --force
```

#### При возникновении чёрного экрана:[](#pri-vozniknovenii-chyornogo-ekrana)

>[!bug] Если по окончании установки и перезагрузки вместо окна входа в систему нас встретит чёрный экран, то в загрузчике добавим через пробел следующие параметры ядра:

```bash
rd.drivers.blacklist=nouveau nouveau.modeset=0
```

>[!info] Также нужно в обязательном порядке зайти в модуль настройки UEFI компьютера или ноутбука и отключить [UEFI Secure Boot](https://ru.wikipedia.org/wiki/Secure_boot) (сама Fedora поддерживает работу с Secure Boot, однако модули ядра проприетарного драйвера не имеют цифровой подписи, поэтому не могут быть загружены в данном режиме и, как следствие, пользователь увидит чёрный экран), а также перевести его из режима **Windows Only** в **Other OS**.

#nvidia