# Подготовка

- Устанавливаем zsh и oh-my-zsh

```bash
sudo apt install zsh

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Тема powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
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
```


# Обновление

```bash
git pull
```


Забираем необходимые конфиги раскладываем по местам:

## alacritty

```bash
## windows
%APPDATA%\alacritty\alacritty.toml

## Linux/Mac os
mkdir -p ~/.config/alacritty
cp alacritty/alacritty.toml ~/.config/alacritty/alacritty.toml
```

## tmux

```bash
# tmux
## Linux
cp tmux/.tmux.conf ~/
```

## zsh

```bash
# zsh
## Linux
cp zsh/.p10k.zsh ~/
cp zsh/.zshrc ~/
```
