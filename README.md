# Подготовка

- Устанавливаем zsh и oh-my-zsh

```bash
sudo apt install zsh

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Тема powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git \
  ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

- Устанавливаем tmux

```bash
sudo apt install tmux
```

- Устанавливаем alacritty

```bash
sudo add-apt-repository ppa:aslatter/ppa
sudo apt install alacritty
```

# Использование

Клонируем репозиторий и создаем symlink(запустив скрипт)

```bash
git clone git@github.com:AKrugRu/workspace.git

cd workspace

sudo chmod +x ./create-ln-dotfiles.sh

./create-ln-dotfiles.sh
```

# Обновление

```bash
git pull

# Если появилась новая ранее не настроенная программа
./create-ln-dotfiles.sh
```
