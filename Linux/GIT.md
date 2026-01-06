### Конфиг

```shell
git config --global --add safe.directory '*'
git config --global user.name "имя"
git config --global user.email "почта"
git config --global credential.helper store
```

### Генерация ключей

```shell
ssh-keygen -t ed25519
mv ~/.ssh/id_ed25519 ~/.ssh/personal_key
mv ~/.ssh/id_ed25519.pub ~/.ssh/personal_key.pub
```

### `~/.ssh/config`

```
Host github.com
    HostName github.com
    User git
    IdentityFile ~/.ssh/personal_key
    IdentitiesOnly yes
```