# vim-setup
## Installation
1. Execute
```
git clone https://github.com/xR3b0rn/vim-setup.git && cp vim-setup/.vimrc ~/.vimrc && sudo rm -r vim-setup && sudo apt-get install -y libncurses-dev && git clone https://github.com/vim/vim.git && cd vim && ./configure --enable-pythoninterp && sudo make -j6 install && cd .. && sudo rm -r vim && git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
2. Open `vim` and execute `:PluginInstall`
