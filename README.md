# vim-setup
## Installation
```
git clone https://github.com/xR3b0rn/vim-setup.git && cp vim-setup/.vimrc ~/.vimrc && sudo rm -r vim-setup && sudo apt-get install -y libncurses-dev && git clone https://github.com/vim/vim.git && cd vim && ./configure --enable-pythoninterp && sudo make -j6 install && cd .. && sudo rm -r vim && git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim && vim -c "PluginInstall" -c "q!"
```

NOTE:
In order to make LSP work properly, in any of the parent directories or the directory of the source file has to be a `compile_commands.json` file, which provides information for `clangd`. This file can be generated e.g. by CMake by setting the `CMAKE_EXPORT_COMPILE_COMMANDS` to ON: `set(CMAKE_EXPORT_COMPILE_COMMANDS ON)` 
