# 2-9-Vim复制粘贴与寄存器的使用.md

## Vim Normal模式复制粘贴
- 复制粘贴分别使用y(yank)和p(ut)
- 剪贴使用d和p
- v模式下选中所要复制的地方，然后使用p粘贴
- yiw复制一个单词，yy复制一行  

## Insert模式下的复制粘贴
- 使用ctr+v 或者cmd+v
- 在vimrc中设置了autoindent，粘贴Python代码缩进错乱, 解决方式:
> :set paste  
:set nopaste

## 什么是Vim的寄存器
- Vim在normal模式下复制/粘贴的内容去哪里了？ 
> Vim操作的是寄存器，而非系统剪切板!!  
默认使用d删除和y复制,x删除的内容都放到了“无名寄存器”  

- 深入寄存器
> Vim使用多组寄存器进行剪贴、复制、粘贴


- 如何使用多组寄存器
> 命令:“regname+cmd, 举例:  
"ayiw 复制一个单词到寄存器a中  
"ap 把寄存器a中的内容粘贴  
“” p其实就等同p  
"+y可以复制到系统剪切板，同理， "+p，可以把系统剪切板内容粘贴到+

- 寄存器和系统剪切板之间互通：
> :set clipboard=unnamed



## 练习文本
> ImageProcessService:  
  buildtype: jarOne   
  build:              
    env:build_args    
      JAVA_HOME: /op  t/soft/openjdk1.8.0_202
  runtime:            
    env:              
      JAVA_HOME: /op  t/soft/jdk
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      bLD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      aLD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
      +LD_PRELOAD: /u  sr/local/lib/libtcmalloc.so
                      
