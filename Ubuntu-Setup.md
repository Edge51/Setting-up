# Setup starts from brand new Ubuntu

## setting path

[environment setting advice](https://stackabuse.com/how-to-permanently-set-path-in-linux/)

zsh is not bash

## remove desktop icons
- home
```
gsettings set org.gnome.shell.extensions.desktop-icons show-home false
```
- trash
```
gsettings set org.gnome.shell.extensions.desktop-icons show-trash false
```
[see also](https://www.omgubuntu.co.uk/2020/03/remove-trash-from-desktop-ubuntu)

## gnome shell extensions
```
sudo apt-get install chrome-gnome-shell
```

## vim
```
sudo apt-get install vim
```
[vundle](https://github.com/VundleVim/Vundle.vim)

## powerline fonts
```
sudo apt-get install fonts-powerlinehttps://linux.wps.com/
```

## zsh
```
sudo apt-get install zsh
chsh -s $(which zsh)
```
#### zsh plugins
- antigen
```
git clone git@github.com:zsh-users/antigen.git
```
and add the following lines to .zshrc ( like vundle to vim ).

```
source /path-to-antigen/antigen.zsh

# Load the oh-my-zsh's library.
antigen use oh-my-zsh

# Bundles from the default repo (robbyrussell's oh-my-zsh).
antigen bundle git
antigen bundle heroku
antigen bundle pip
antigen bundle lein
antigen bundle command-not-found

# Syntax highlighting bundle.
antigen bundle zsh-users/zsh-syntax-highlighting

# Load the theme.
antigen theme robbyrussell

# Tell Antigen that you're done.
antigen apply
```
Additionally, I set the bundle directory manually by changing the default directory environment in antigen.zsh

[more informations](https://github.com/zsh-users/antigen)

## git
```
sudo apt-get install git
```

## Chinese display support

```
sudo apt-get install language-pack-zh*
sudo apt-get install chinese*
https://linux.wps.com/
sudo locale-gen en_GB.UTF-8
sudo update-locale LANG=en_GB.UTF-8
```

## markdown to pdf support
- pandoc and grip with chromium
  - for outputting pdf from markdown


## birdtray
```
sudo apt-get install birdtray
```

## chromium
```
sudo apt-get install chromium-browser
```

## language
[manage in this way](https://help.ubuntu.com/lts/ubuntu-help/prefs-language-install.html.en)

## keyboard shortcut remap
settings-->keyboard shortcuts

|descriptions|shortcuts|
| -------- |---------|
|switch windows of an application|alt + `|
|switch applications|alt + tab|

## python
currently use the python3 installed by default.
- install pip
```
sudo apt-get install python3-pip
```
- install numpy
```
sudo apt-get install python3-numpy
```
## abobe flash player
for videos on firefox
```
sudo apt-get install flashplugin-installer
```
## enable videos
```
sudo apt install libavcodec-extra
```

## vscode
install by deb downloaded from official website.

keyboard mapping
|fuction|shortcuts|
|-----|-----|
|activity bar|ctrl+'|

## Chinese input method
install sogoupinyin by deb downloaded from official website
```
sudo apt-get install fcitx
im-switch -s fcitx
```

## hide bars
- ubuntu top bar
```
sudo apt install gnome-shell-extension-autohidetopbar
```
- title bar

```
sudo apt-get install gnome-shell-extension-pixelsaver
gsettings set org.gnome.Terminal.Legacy.Settings headerbar false
```

## simplenote
install by deb downloaded from official website

## for github
```
sudo apt-get install xclip
```

## curl
```
sudo apt-get install curl
```

## latex install
```
sudo apt-get install texlive-full
```

## octave
```
sudo apt-get install octave
sudo apt-get install octave-control octave-image octave-io octave-optim octave-signal octave-statistics
```

## gimp
```
sudo apt-get install gimp
```

## QQ
[install from .deb](https://im.qq.com/linuxqq/index.html)

## totem ( video player)( purged, use vlc instead)
```
sudo apt-get install totem
```

## vlc ( video player )
```
sudo apt-get install vlc
```

## transmission
```
sudo apt-get install transmission
```

## dia (diagram creation program)
```
sudo apt-get install dia
```

## dosbox ( course lab required )
```
sudo apt-get install dosbox
```

## nasm ( assembly language required )
```
sudo apt-get install nasm
```

## wps
[installed by deb](https://linux.wps.com/)

## mysql
```
sudo apt install mysql-client-core-8.0
```
