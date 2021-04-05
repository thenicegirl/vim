# How to use vim-plug
https://github.com/junegunn/vim-plug

curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

# How to find plugin
* Google
*   vim file manager plugin
*   vim python plugin github
* VimAwesome
* Try other's vimrc

# Plugin recommand

* mhinz/vim-startify
* vim-airline/vim-airline
* Yggdroot/indentLine

# Theme recommand

* w0ng/vim-hybrid
* altercation/vim-colors-solarized
* morhetz/gruvbox

# Other
* preservim/nerdtree
  * ![image](https://user-images.githubusercontent.com/53411757/113613486-e31ad200-9683-11eb-98c4-e1110fe7d2c5.png)

* kien/ctrlp.vim
  * tornadowebpy

* easymotion/vim-easymotion
  * ss
  * ...

* tpope/vim-surround
  * ds delete a surrounding
  * cs change a surrounding
    * cs " '
    * cs ( ]
  * ys you add a surrounding
    * ys iw "

* Ag.vim / fzf.vim
* junegunn/fzf.vim
  * :Files .
  * :Ag duck
  * ctrl j/k

* brooth/far.vim
* :Far gua ga **/*
* :Fardo

* Plug 'fatih/vim-go', { 'do': ':GoUpdateBinaries' }
  * ctrl x o
  * ctrl ]
  * ctrl o / i
  * :GoFmt
  * :GoRename
  * :GoImports
  * :GoRun

* jedi-vim / python-mode
* Plug 'python-mode/python-mode', { 'for': 'python', 'branch': 'develop' }
  * ![image](https://user-images.githubusercontent.com/53411757/113624119-ceddd180-9691-11eb-97ed-b83e5a0c20c7.png)
  * ctrl c ro
  * :PymodeLintAuto
