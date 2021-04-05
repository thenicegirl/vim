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
```vim
" 常用设置
" 设置行号
set number
colorscheme hybrid
" 按F2进入粘贴模式
set pastetoggle=<F2>
" 高亮搜索
set hlsearch
" 设置折叠方式
set foldmethod=indent

" 一些方便的映射
let mapleader=','
1et g:mapleader=','

" 使用jj进入normal模式
inoremap jj <Esc>`^
" 使用leader+w直接保存
inoremap <leader>w <Esc>:w<cr>
noremap <leader>w :w<cr>

" 切换buffer
nnoremap <silent> [b :bprevious<CR>
nnoremap <silent> [n :bnext<CR>
" use ctrl+h/j/k/l switch window
noremap <C-h> <C-w>h
noremap <C-j> <C-w>j
noremap <C-k> <C-w>k
noremap <C-l> <C-w>l

"Sudo to write
cnoremap w!! w !sudo tee %>/dev/null
"json 格式化
com! FormatJSON %!python3 -m json.tool

“插件设置，这里使用了vim-plug call plug#begin（'~/.vim/plugged'）
“安装插件只需要把github地址放到这里重启后执行：币1ugInstal1就好了
Plug'mhinz/vim-startify'
Plug'scrooloose/nerdtree'
cal1 plug#end）
![image](https://user-images.githubusercontent.com/53411757/113611464-21fb5880-9681-11eb-8d81-2a2c6621f8d9.png)
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
