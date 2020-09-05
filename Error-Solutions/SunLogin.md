Sunlogin error solution
=======

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
