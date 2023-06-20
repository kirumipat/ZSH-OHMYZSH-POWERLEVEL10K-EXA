# ZSH OHMYZSH POWERLEVEL10K EXA
<img src="https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/extravagant-style.png">


## Нужный шрифт - FiraCode NF
```console
https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraCode
```
## Сам шрифт
```console
https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/FiraCode/Medium/complete/Fira%20Code%20Medium%20Nerd%20Font%20Complete.ttf
```
## Установите пакет ZSH

## ARCH ----->[<img src="https://cdn0.iconfinder.com/data/icons/flat-round-system/512/archlinux-512.png" width="50" height="50" >](https://archlinux.org/download/)
```console
sudo pacman -Sy zsh zsh-completions
```
## UBUNTU -->[<img src="https://brandslogos.com/wp-content/uploads/images/large/ubuntu-logo.png" width="50" height="50" >](https://ubuntu.com/)
```console
sudo apt-get install zsh -y
```
## FEDORA --->[<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Fedora_logo.svg/1024px-Fedora_logo.svg.png" width="50" height="50" >](https://getfedora.org/)
```console
sudo dnf install zsh
```
## Установить ZSH по умолчанию
```console
sudo chsh -s /bin/zsh 
```
## После переходим к настройкам

## Install Oh My Zsh
```console
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
## Install PowerLevel10k
```console
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
## Установка темы
```console
sudo nano ~/.zshrc
```
```console
ZSH_THEME="powerlevel10k/powerlevel10k"
```
## Если после перезагрузки настройки не включились автоматически введите команду
```console
p10k configure
```
# Плагины

## Подсветка синтаксиса
```console
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
## Авто дополнение
```console
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
## Включаем плагины
```console
sudo nano ~/.zshrc
```
```console
plugins=( git zsh-syntax-highlighting zsh-autosuggestions )
```
# Замена стандартных команд

## ls - установите пакет ```exa```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
if [ -x "$(command -v exa)" ]; then
    alias ls="exa --long --all --group"
fi
```
## cat - установите пакет ```bat```
откройте настройки шэла 
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias cat="bat"
```
## df - установите пакет ```duf```
откройте настройки шэла 
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias df="duf"
```
## find - установите пакет ```fd```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias find="fd"
```
## man - установите пакет ```tldr```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias man="tldr"
```
## top - установите пакет ```btop```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias top="btop"
```
## du - установите пакет ```ncdu```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias du="ncdu"
```
## ping - установите пакет ```gping```
откройте настройки шэла
```console
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```console
alias ping="gping"
```

# Включить подсветку в ```nano```
```console
nano ~/.nanorc
```
```console
include /usr/share/nano/*.nanorc
```

# Плагины [OHMYZSH](https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins)


## VIDEO
[<img src="https://i.ytimg.com/vi/yfq1H9bT8c4/maxresdefault.jpg" width="600" height="400" >](https://youtu.be/yfq1H9bT8c4)
