# ZSH-OHMYZSH-POWERLEVEL10K-EXA



Нужный шрифт - FiraCode NF
Установите пакет ZSH 
После переходим к настройкам

Install Oh My Zsh -  
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Install PowerLevel10k -  
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k

Установка темы -   sudo nano ~/.zshrc
ZSH_THEME="powerlevel10k/powerlevel10k"
Если после перезагрузки настройки не включились автоматически введите команду - 
p10k configure

Плагины
Подсветка синтаксиса
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
Авто дополнение
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

Замена стандартных команд

ls - установите пакет exa
откройте настройки шэла - sudo nano ~/.zshrc
добавьте в самый низ эти строки
if [ -x "$(command -v exa)" ]; then
    alias ls="exa"
    alias la="exa --long --all --group"
fi

cat - установите пакет bat
откройте настройки шэла - sudo nano ~/.zshrc
добавьте в самый низ эти строки
alias cat="bat"

df - установите пакет duf
откройте настройки шэла - sudo nano ~/.zshrc
добавьте в самый низ эти строки
alias df="duf"

find - установите пакет fd
откройте настройки шэла - sudo nano ~/.zshrc
добавьте в самый низ эти строки
alias find="fd"

man - установите пакет tldr
откройте настройки шэла - sudo nano ~/.zshrc
добавьте в самый низ эти строки
alias man="tldr"
