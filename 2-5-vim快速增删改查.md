# 2-5-Vim快速增删改查.md

## 增加字符
a,i,o,A,I,O 6个字母，6中插入方式

## 快速删除
**normal 模式下**
- x 快速删除一个字符
- d 配合文本对象快速删除一个单词 daw(delete a word)
- dd 删除一行
- d + $/0，快速删除光标到行尾/行首
- d + )/"/} ，快速删除到 ) 或者 “ 或者} 之间的内容
- x 或者 d , 配合数字可以删除多个字符/行 ，如4x 或者 4dd
- daw ,删除一个单词

**visual 模式下**
- 基本可以参考nomal模式下的命令

## 快速修改
**常用的有3个，r-replace, c-change, s-substitute**
- r+字符，替换光标所在的字符 
- 数字n+r+字符a，将光标所在字符后面n个字符同时替换为字符a
- c+字符
- c+字符, 删除当前字符并进入插入模式
- c+w, 删除当前单词并进入插入模式
- c+ )或者“ 或者] 或者 },直接删除到对应的符号
- caw，删除一个单词,并进入插入模式

## 查询
- 使用/ 或者 ？进行前向或者反向搜索
- 使用n/N跳转到下一个或者上一个匹配

> Text Example1
It is a nice nice nice nice day, I very happy happy happy  happy.
Monday 
Monday 
Tuesday 
.
 , tts, car, dog, egg, food,   asdfgoods,
Tuesday 
.
abcdon , tts, car, dog, egg, food,   asdfgoods,
It 
Mon
Tue
Jul
Jun
abc
