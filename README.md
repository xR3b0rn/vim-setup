# vim-setup
## Installation
1. Install libncurses-dev: `sudo apt-get install -y libncurses-dev`
2. Clone the most current version of `vim` from https://github.com/vim/vim (`git clone https://github.com/vim/vim.git`), configure it with `./configure --enable-pythoninterp` and build and install it with `make -j6 install`
3. Install the plugin manager `Vundle` with `git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
4. Copy `.vimrc` to `~/.vimrc`
5. Open `vim` and execute `:PluginInstall`

Step 1-3:
```
sudo apt-get install -y libncurses-dev && git clone https://github.com/vim/vim.git && cd vim && ./configure --enable-pythoninterp && sudo make -j6 install && cd .. && rm -r vim && git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
