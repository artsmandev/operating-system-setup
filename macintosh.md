<!--
  MIT License

  Copyright (c) 2020 Bruno Andrade

  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:

  The above copyright notice and this permission notice shall be included in all
  copies or substantial portions of the Software.

  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
-->

# homebrew
  * /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
  * in case of problem when download XCode Command Line Tools, get it directly: https://developer.apple.com/download/more/
  * brew analytics off

# xcode command line tools
 * xcode-select --install

# iterm2
  * brew cask install iterm2

# git
  * brew install git

# vim
  * brew install vim

# zsh
  * brew install zsh
  * chsh -s /bin/zsh

# ohmyzsh
  * sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

# powerlevel10k
  * git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
  * cd $(echo $ZSH)/custom/plugins \
      && git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
      && git clone https://github.com/zsh-users/zsh-autosuggestions.git
  * vim ~/.zshrc
      * ZSH_THEME=powerlevel10k/powerlevel10k
      * plugins=(git zsh-syntax-highlighting zsh-autosuggestions)
  * In case of problems with font's icons
      * https://github.com/Powerlevel9k/powerlevel9k/wiki/Install-Instructions
      * https://github.com/ryanoasis/nerd-fonts (Hack Regular Nerd Font Complete Mono)

# curl
  * brew install curl

# wget
  * brew install wget

# nmap
  * brew install nmap

# speedtest
  * brew install speedtest-cli

# translate-shell
  * brew install translate-shell

# mvn
  * brew install maven

# gradle
  * brew install gradle

# intellij idea:
  * brew cask install intellij-idea

# dbeaver
  * brew cask install dbeaver-community

# docker
  * brew cask install docker

# vscode
  * brew cask install visual-studio-code

# dashlane
  * brew cask install dashlane

# verarcrypt
  * brew cask install veracrypt

# whatsapp
  * brew cask install whatsapp

# postman
  * brew cask install postman

# vlc
  * brew cask install vlc

