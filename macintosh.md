# homebrew
  * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
  * in case of problem when download XCode Command Line Tools, get it directly: https://developer.apple.com/download/more/
  * brew analytics off

# xcode command line tools
 * xcode-select --install

# iterm2
  * brew install --cask iterm2

# git
  * brew install git
  * export LESS=Rx4

# vim
  * brew install vim

# zsh
  * brew install zsh
  * chsh -s /bin/zsh

# ohmyzsh
  * sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

# powerlevel10k
  * git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
  * cd $(echo $ZSH)/custom/plugins \\  
      && git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \\  
      && git clone https://github.com/zsh-users/zsh-autosuggestions.git
  * sed -i '' 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc
  * sed -i '' 's/plugins=(git)/plugins=(git zsh-syntax-highlighting zsh-autosuggestions)/' ~/.zshrc
  * brew tap homebrew/cask-fonts
  * brew install --cask font-hack-nerd-font

# curl
  * brew install curl
  * echo 'export PATH="/opt/homebrew/opt/curl/bin:$PATH"' >> ~/.zshrc

# wget
  * brew install wget

# nmap
  * brew install nmap

# speedtest
  * brew install speedtest-cli

# translate-shell
  * brew install translate-shell

# sdkman
  * curl -s "https://get.sdkman.io" | bash
  * source "/Users/bruno/.sdkman/bin/sdkman-init.sh"

# jdk
  * sdk install java 21-tem

# mvn 
  * sdk install maven 3.9.5

# gradle
  * brew install gradle 8.4

# jq
  * brew install jq

# httpie
  * brew install httpie

# intellij idea:
  * brew install --cask intellij-idea

# vscode
  * brew install --cask visual-studio-code

# docker
  * brew install --cask docker
  * brew install docker-compose

# colima
  * brew install colima

# postman
  * brew cask install postman

# dbeaver
  * brew cask install dbeaver-community

# whatsapp
  * brew cask install whatsapp

# vlc
  * brew cask install vlc

# gitkraken
  * brew cask install gitkraken

