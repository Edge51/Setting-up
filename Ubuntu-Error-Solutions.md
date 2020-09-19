Ubuntu Error Solutions
=======

## ReText

the default ReText does not display math formula.

to enable math formula display:
```
sudo apt-get install libjs-mathjax
```

“Edit → Use WebKit renderer”

## Sunlogin error solution

dependency Package libwebkitgtk-3.0-0 is not installed.
add following line to /etc/apt/sources.list
```
deb http://cz.archive.ubuntu.com/ubuntu bionic main universe
```

then run following line in terminal
```
sudo apt --fix-broken install
```

to enable windows player to login ubuntu use the lightdm.(the default one is gdm3 before)
```
sudo apt-get install lightdm
```

## duplicated icons
I installed visual studio code before, and remove it later. However, when I type code in activity, the icon still shows.
To solve this problem
> remove relative icon in ~/.local/share/applications/*.desktop.

## vim

### 1

fatal: unable to access 'https://github.com/whqee/whqee.github.git/': Failed to connect to 127.0.0.1 port 1080: 拒绝连接

git config --global http.proxy 'socks5://127.0.0.1:1080'

### 2

ycm_core = ImportCore()
  File "/home/edge51/.vim/bundle/YouCompleteMe/third_party/ycmd/ycmd/utils.py", line 489, in ImportCore
  import ycm_core as ycm_core
ImportError: libpython3.7m.so.1.0: cannot open shared object file: No such file or directory

python2 not available anymore

python3 install.py
