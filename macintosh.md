# xcode command line tools
 * xcode-select --install
 * in case of problem when download XCode Command Line Tools, get it directly: https://developer.apple.com/download/more/

# homebrew
  * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
  * brew analytics off

# iterm2
  * brew install --cask iterm2

# zsh
  * brew install zsh
  * chsh -s /bin/zsh
  * echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zshrc

# ohmyzsh
  * sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

# git
  * brew install git
  * brew link --overwrite git
  * echo 'export LESS=Rx4' >> ~/.zshrc
  * git config --global user.name
  * git config --global user.email

# powerlevel10k
  * git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
  * cd $(echo $ZSH)/custom/plugins \\  
      && git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \\  
      && git clone https://github.com/zsh-users/zsh-autosuggestions.git
  * sed -i '' 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\\/powerlevel10k"/' ~/.zshrc
  * sed -i '' 's/plugins=(git)/plugins=(git zsh-syntax-highlighting zsh-autosuggestions)/' ~/.zshrc
  * brew install --cask font-hack-nerd-font

# vim
  * brew install vim

# gpg
  * brew install gpg
  * gpg --full-generate-key
  * gpg --list-secret-keys --keyid-format=long
  * gpg --armor --export _[key]_
  * git config --global user.signingkey _[key]_
  * git config --global commit.gpgsign true

# ssh
  * ssh-keygen -t ed25519 -C "email"
  * eval "$(ssh-agent -s)"
  * ssh-add --aple-use-keychain ~/.ssh/id_id25519

# curl
  * brew install curl
  * echo 'export PATH="/opt/homebrew/opt/curl/bin:$PATH"' >> ~/.zshrc
  * echo 'export LDFLAGS="-L/opt/homebrew/opt/curl/lib"' >> ~/.zshrc
  * echo 'export CPPFLAGS="-I/opt/homebrew/opt/curl/include"' >> ~/.zshrc

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
  * sdk install java 22.0.2-tem

# mvn 
  * sdk install maven 3.9.8

# gradle
  * brew install gradle 8.10

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
  * colima start --cpu 2 --menory 6
  * echo 'export DOCKER_HOST=unix://$HOME/.colima/default/docker.sock' >> ~/.zshrc
  * add `"cliPluginsExtraDirs": [ "/opt/homebrew/lib/docker/cli-plugins" ]` into ~/.docker/config.json

# caffeine
  * brew install caffeine

# rectangle
  * brew install --cask rectangle

# postman
  * brew install --cask postman

# dbeaver
  * brew install --cask dbeaver-community

# vlc
  * brew install --cask vlc

# gitkraken
  * brew install --cask gitkraken

# firefox
  * brew install --cask firefox@developer-edition

# chrome
  * brew install --cask google@chrome
