# Подготовка

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
