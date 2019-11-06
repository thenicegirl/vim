#  2-7-Vim多文件操作.md

## 多文件操作的相关概念
- Buffer, 指打开的一个文件的内存缓冲区
- 窗口，是Buffer可视化的分割区域
- Tab

## Buffer 切换
- :ls 列举当前缓冲区，然后使用 :b n 跳转到第n个缓冲区
- :bpre, :bnext，:bfirst, :blast
- :e ./文件名，可以在当前窗口打开新的文件
- :bNext, 跳转到下一个文件

## Window 窗口
- 一个缓冲区可以分割成多个窗口，每个窗口可以打开不同的缓冲区
- :sp 水平分割
- :vs 垂直分割

## Tab
- 在Window窗口，:tabnew fileName，可以新建tab页并且打开新文件
- gt 在多个窗口之间切换
- tabc[close] ,关闭当前tab页
- tabo[nly] ，只保留当前页
