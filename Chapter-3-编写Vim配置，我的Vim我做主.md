# Linux/Unix
touch ~/.vimrc

# Windows
vim $MYVIMRC

# Activate vimrc
1. Quit and reopen
2. :source ~/.vimrc

# Example

```vim
set number
syntax on
```
ZZ save & quit

:h option-list
```vim
set number
colorscheme hybrid
set pastetoggle=<F2>  " Press F2 to paste mode
set hlsearch  " highlight search
set foldmethod=indent

let mapleader=','
let g:mapleader=','

" inoremap
" i insert
" nore no recursive
" map

inoremap jj <Esc>`^  " Type jj to normal mode
inoremap <leader>w <Esc>:w<cr>  " Type ,w save directly
noremap <leader>w :w<cr>

" Switch buffer
nnoremap <silent> [b :bprevious<CR>
nnoremap <silent> [n :bnext<CR>
" Use ctrl+h/j/k/l switch window
noremap <C-h> <C-w>h
noremap <C-h> <C-w>j
noremap <C-h> <C-w>k
noremap <C-h> <C-w>l

" Sudo to write
cnoremap w!! w !sudo tee % >/dev/null
" json Format
com! FormatJSON %!python3 -m json.tool

" Set plugin
call plug#begin('~/.vim/plugged')

Plug 'mhinz/vim-startify'
Plug 'scrooloose/nerdtree'

call plug#end()

" About plugin
let g:startify_change_to_dir = 0  # Ban startify auto switch dir

" nerdtree
nmap ,v :NERDTreeFind<cr>
nmap ,g :NERDTreeToggle<cr>


" Define SetTitle function, auto insert file head
func SetTitle()
  if &filetype == 'python'
    call setline(1, "\#!/usr/bin/env python")
    call setline(2, "\# -*- coding:utf-8 -*-")
    normal G
    normal o
    normal o
    call setline(5, "if __name__ == '__main__':")
    call setline(6, "  pass")
  endif
endfunc
```

# Vim map
## Not recommanded
:map - x
:map `<space>` viw
:map `<c-d>` dd
:unmap -

* nmap
* vmap
*   :vmap \ U
* imap
*   :imap <c-d> <Esc>ddi
* 

## Recommanded
* nnoremap
* vnoremap
* inoremap
* 
