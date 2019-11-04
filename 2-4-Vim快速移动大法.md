# 字符之间移动:

     ^
     k

<h   .   l>

     j
     v


# 单词之间“飞舞”
w/W 移动到下一个word/Word开头，e/E 下一个word/WORD结尾;
b/B 回到上一个work/WORD开头，理解为backWord.
(word 是以非空白符分割的单词，WORD是以空白符分割的单词.)

Example TEXT:
Hello world, i am Sai. It is a test text.
Today is Monday, the day is 4th Nov 2019. I am from China. BeiJing is a beautiful city. My MacBook is ￥15000. WOW!      

# 行间搜索移动
* f{char},可以移动到char字符上，t移动到char字符的前一个字符
分号(;) 逗号(,) 继续搜索当前行的下一个/上一个字符
* 大写F，表示反过来搜索前面的字符

# 水平移动
0，移动到行首第一个字符
$，移动到行尾

# 页面移动
gg/G 移动到文件开头和结尾，
H/M/L 跳转到屏幕的开头-HEAD, 中间-Middle, 结尾Lower
ctrl+f, ctrl+b，上下翻页
zz，把当前行放到中间.
