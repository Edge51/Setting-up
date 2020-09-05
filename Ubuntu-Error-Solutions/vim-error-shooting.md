# 1

fatal: unable to access 'https://github.com/whqee/whqee.github.git/': Failed to connect to 127.0.0.1 port 1080: 拒绝连接

git config --global http.proxy 'socks5://127.0.0.1:1080'

# 2

ycm_core = ImportCore()
  File "/home/edge51/.vim/bundle/YouCompleteMe/third_party/ycmd/ycmd/utils.py", line 489, in ImportCore
  import ycm_core as ycm_core
ImportError: libpython3.7m.so.1.0: cannot open shared object file: No such file or directory

python2 not available anymore

python3 install.py
