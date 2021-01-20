## neofetch:
  * sudo apt install neofetch -y

## curl:
  * echo deb http://ppa.launchpad.net/savoury1/curl34/ubuntu $(lsb_release -cs) main \
      | sudo tee /etc/apt/sources.list.d/curl.list
  * sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 374C7797FB006459
  * sudo apt upgrade -y && sudo apt install curl -y

## vim:
  * echo deb http://ppa.launchpad.net/jonathonf/vim-daily/ubuntu $(lsb_release -cs) main \
      | sudo tee /etc/apt/sources.list.d/vim.list
  * sudo apt install vim -y

## git:
  * echo deb http://ppa.launchpad.net/git-core/ppa/ubuntu $(lsb_release -cs) main \
    | sudo tee /etc/apt/sources.list.d/git.list
  * sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 8CF63AD3F06FC659
  * sudo apt update && sudo apt install git -y

## zsh:
  * sudo apt install zsh -y

## ohmyzsh:
  * sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  * cd $(echo $ZSH)/custom/plugins \
      && git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
      && git clone https://github.com/zsh-users/zsh-autosuggestions.git
  * cd $(echo $ZSH)/custom/themes \
      && git clone --depth=1 https://github.com/romkatv/powerlevel10k.git
  * vim ~/.zshrc
      * change theme to: ZSH_THEME=powerlevel10k/powerlevel10k
      * change plugins to: plugins=(git zsh-syntax-highlighting zsh-autosuggestions)
  * Download Hack Regular Nerd Font Complete Mono in the
      * https://github.com/ryanoasis/nerd-fonts
      * https://github.com/Powerlevel9k/powerlevel9k/wiki/Install-Instructions (in case of problem)

## tilix:
  * sudo apt install tilix -y
  * sudo update-alternatives --config x-terminal-emulator

## translate-shell
  * sudo apt install translate-shell -y

## nmap
  * sudo apt install nmap -y

## docker
  * sudo apt remove --purge docker docker-engine docker.io containerd runc
  * sudo apt install \
      apt-transport-https \
      ca-certificates \
      curl \
      gnupg-agent \
      software-properties-common
  * curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
  * sudo apt-key fingerprint 0EBFCD88
  * sudo add-apt-repository \
      "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
      $(lsb_release -cs) stable" //or focal stable"
  * sudo apt-get install docker-ce docker-ce-cli containerd.io -y
  * sudo groupadd docker, only if already not exists
  * newgroup docker

## vscode
  * snap install code --classic

## sdkman
  * curl -s "https://get.sdkman.io" | zsh

## maven
  * sudo apt install maven -y

## intellij
  * snap install intellij-idea-ultimate --classic

## postman
  * snap install postman --classic

## dbeaver
  ** snap install dbeaver --classic

## vlc
  * snap install vlc --classic
