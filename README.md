# bash setup

## brew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew install wget

### brew tap channels
brew tap brewsci/science
brew tap brewsci/bio

## git 
### git autocompletion
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash

### git open
npm install --global git-open

## oh-my-zsh
sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"

git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions

### power level 9k theme
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k

### terminal themes:
https://github.com/lysyi3m/osx-terminal-themes

## Powerline
pip install --user powerline-status

brew install macvim --env-std --with-override-system-vim

### Powerline font
git clone https://github.com/powerline/fonts.git

cd fonts

./install.sh

cd ..

rm -rf fonts

### Awesome Powerline font
https://github.com/gabrielelana/awesome-terminal-fonts

## fish
brew install fish

echo "/usr/local/bin/fish" | sudo tee -a /etc/shells

chsh -s /usr/local/bin/fish

curl -L https://get.oh-my.fish | fish

## imgcat
brew tap eddieantonio/eddieantonio

brew install imgcat 

## screenfetch
brew install screenfetch 



## Software

### Papers
http://papersapp.com/mac/

### QQ browser
http://bbs.browser.qq.com/thread-92391-1-1.html

### Atom
https://atom.io/

### Anaconda
https://www.continuum.io/downloads

## Slack
* Druckmannlab
* ahrenslab
* pixybot
* mesoscaleactivitymap
* mlreadingclub

## Remove guest account at login

sudo defaults write /Library/Preferences/com.apple.loginwindow SHOWOTHERUSERS_MANAGED -bool FALSE


## MacOSX
### rebuild spotlight

sudo mdutil -E /
