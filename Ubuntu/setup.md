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

## zsh
```
sudo apt-get install zsh
chsh -s $(which zsh)
```

## git
```
sudo apt-get install git
```

## Chinese display support

```
sudo apt-get install language-pack-zh*
sudo apt-get install chinese*

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
## abobe flash player
for videos on firefox
```
sudo apt-get install flashplugin-installer
```
