```bash
sudo dnf install zsh

sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"

sudo usermod USER -s /bin/zsh

sudo dnf -y install google-noto-emoji-fonts

git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Добавить `ZSH_THEME="powerlevel10k/powerlevel10k"` в `~/.zshrc`
