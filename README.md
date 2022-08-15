# ZSH-OHMYZSH-POWERLEVEL10K-EXA

## Нужный шрифт - FiraCode NF
```zsh
https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraCode
```
## Сам шрифт
```
https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/FiraCode/Medium/complete/Fira%20Code%20Medium%20Nerd%20Font%20Complete.ttf
```
## Установите пакет ZSH

## ARCH
```bash
sudo pacman -Sy zsh zsh-completions
```
## UBUNTU
```bash
sudo apt-get install zsh -y
```
## FEDORA
```bash
sudo dnf install zsh
```
## Установить ZSH по умолчанию
```bash
sudo chsh -s /bin/zsh 
```
## После переходим к настройкам

## Install Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
## Install PowerLevel10k
```bash
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
## Установка темы
```bash
sudo nano ~/.zshrc
```
```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```
## Если после перезагрузки настройки не включились автоматически введите команду - 
```bash
p10k configure
```
# Плагины

## Подсветка синтаксиса
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
## Авто дополнение
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
# Замена стандартных команд

## ls - установите пакет ```exa```
откройте настройки шэла
```bash
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
if [ -x "$(command -v exa)" ]; then
    alias ls="exa"
    alias la="exa --long --all --group"
fi
```
## cat - установите пакет bat
откройте настройки шэла 
```bash
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
alias cat="bat"
```
## df - установите пакет duf
откройте настройки шэла 
```bash
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
alias df="duf"
```
## find - установите пакет fd
откройте настройки шэла
```bash
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
alias find="fd"
```
## man - установите пакет tldr
откройте настройки шэла
```bash
sudo nano ~/.zshrc
```
добавьте в самый низ эти строки
```bash
alias man="tldr"
```
## VIDEO

[![INSATALL ADDGUARD HOME](https://i.ytimg.com/vi/yfq1H9bT8c4/hqdefault.jpg)](https://youtu.be/A4FTz2vLCMo)
