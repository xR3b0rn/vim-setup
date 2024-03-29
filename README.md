# vim-setup
## Installation
```
git clone https://github.com/xR3b0rn/vim-setup.git && cp vim-setup/.vimrc ~/.vimrc && sudo rm -r vim-setup && sudo apt-get install -y libncurses-dev python3.10 && git clone https://github.com/vim/vim.git && cd vim && sudo add-apt-repository ppa:deadsnakes/ppa && sudo apt-get install -y python3.11 libpython3.11-dev && ./configure --enable-python3interp --with-python3-command=/usr/bin/python3.11 && sudo make -j6 install && cd .. && sudo rm -r vim && git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim && vim -c "PluginInstall" -c "q!" -c "q!"
```

NOTE two things:
* For the first time editing a source file of a certain language, the command `:LspInstallServer` has to be executed in `vim` to install the needed language server. Execute `:LspUninstallServer server-name` to uninstall the language server. 
* In order to make LSP work properly, in any of the parent directories or the directory of the source file has to be a `compile_commands.json` file, which provides information for `clangd`. This file can be generated e.g. by CMake by setting the `CMAKE_EXPORT_COMPILE_COMMANDS` to ON: `set(CMAKE_EXPORT_COMPILE_COMMANDS ON)` 
