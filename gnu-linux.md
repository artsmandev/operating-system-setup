## neofetch:
```
sudo apt install neofetch -y
```

## curl:
```
echo "deb http://ppa.launchpad.net/savoury1/curl34/ubuntu $(lsb_release -cs) main" \
  | sudo tee /etc/apt/sources.list.d/curl.list &&\
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 374C7797FB006459 &&\
sudo apt update && sudo apt install curl -y
```

## vim:
```
sudo apt install vim -y
```

## git:
```
echo deb http://ppa.launchpad.net/git-core/ppa/ubuntu $(lsb_release -cs) main \
  | sudo tee /etc/apt/sources.list.d/git.list &&\
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys A1715D88E1DF1F24 &&\
sudo apt update && sudo apt install git -y &&\
git --version
```

## zsh:
```
sudo apt install zsh -y
```

## ohmyzsh:
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
cd $(echo $ZSH)/custom/plugins &&\
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git &&\
  git clone https://github.com/zsh-users/zsh-autosuggestions.git &&\
cd $(echo $ZSH)/custom/themes &&\
  git clone --depth=1 https://github.com/romkatv/powerlevel10k.git && cd ~ &&\
sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc &&\
sed -i 's/plugins=(git)/plugins=(git zsh-syntax-highlighting zsh-autosuggestions)/' ~/.zshrc &&\
mkdir ~/.fonts &&\
  curl https://raw.githubusercontent.com/ryanoasis/nerd-fonts/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete%20Mono.ttf -o ~/.fonts/hack-regular-nerd-font-complete-mono.ttf &&\
source ~/.zshrc
```

## tilix:
```
sudo apt install tilix -y &&\
sudo update-alternatives --config x-terminal-emulator
```
  * Global
    * 3, 5, 6, 7, 10 and 12
  * Appearance
    * Disable CSD, hide toobar
    * Small
    * 4 and 5
    * Quake
      * Size: 40 x 05
      * Options
        * 1, 3, 4, and 5

## translate-shell
```
sudo apt install translate-shell -y
```

## nmap
```
sudo apt install nmap -y
```

## docker
```
sudo apt remove --purge docker docker.io containerd runc &&\
sudo apt install \
  apt-transport-https \
  ca-certificates \
  curl \
  gnupg-agent \
  software-properties-common -y &&\
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - &&\
sudo apt-key fingerprint 0EBFCD88 &&\
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" &&\
sudo apt install docker-ce docker-ce-cli containerd.io -y &&\
sudo usermod -aG docker $(whoami) &&\
  newgrp docker
```

## vscode
```
snap install code --classic
```

## sdkman
```
curl -s "https://get.sdkman.io" | zsh
```

## maven
```
sudo apt install maven -y
```

## intellij
```
snap install intellij-idea-ultimate --classic
```

## postman
```
snap install postman --classic
```

## dbeaver
```
snap install dbeaver-ce --classic
```

## mpv
```
sudo apt install mpv -y
```

## flameshot
```
snap install flameshot --classic
```

## tweaks
```
sudo apt install gnome-tweaks -y
```

## spotify
```
snap install spotify
```

## gitkraken
```
snap install gitkraken --classic
```

## firefox
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys A6DCF7707EBC211F &&\
  echo "deb [arch=amd64] http://ppa.launchpad.net/ubuntu-mozilla-security/ppa/ubuntu $(lsb_release -cs) main" \
    | sudo tee /etc/apt/sources.list.d/firefox.list &&\
sudo apt update && sudo apt upgrade -y
```

## speedtest
```
sudo apt install gnupg1 apt-transport-https dirmngr -y &&\
  sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61 &&\
echo "deb [arch=amd64] https://ookla.bintray.com/debian generic main" \
  | sudo tee /etc/apt/sources.list.d/speedtest.list
sudo apt update && sudo apt upgrade && sudo apt install speedtest -y
```

## google chrome
```
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - &&\
  echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" \
    | sudo tee /etc/apt/sources.list.d/google-chrome.list &&\
sudo apt update && sudo apt install google-chrome-stable -y
```

## slack
```
snap install slack --classic
```

## gnome extensions

  * https://extensions.gnome.org/extension/7/removable-drive-menu/
  * https://extensions.gnome.org/extension/906/sound-output-device-chooser/
  * https://github.com/paradoxxxzero/gnome-shell-system-monitor-applet
  * https://extensions.gnome.org/extension/750/openweather/
  * https://extensions.gnome.org/extension/2603/spotify-label/