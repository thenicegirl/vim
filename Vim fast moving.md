> Standing on the shore can't learn to swim, Studying without practice can't learn Vim

# Vim fast moving

## Move between characters:
          ^
          k         
      <h  .  l>
          j
          v

## Move between characters:
- `w` / `W` Move to the beginning of the next word/Word
- `e` / `E` Move to the end of next word/WORD
- `b` / `B` Go back to the beginning of the previous work/WORD, understood as backWord.
- (word is a word separated by non-white space, WORD is a word separated by white space.)

- Example TEXT:  
Hello world, i am Sai. It is a test text.  
Today is Monday, the day is 4th Nov 2019. I am from China. BeiJing is a beautiful city. My MacBook is ￥15000. WOW!      

## Search and move between lines
* `f{char}` Move to {char} character，
* `t{char}` Move to the previous character of {char}
* Semicolon (;) Comma (,) Continue to search for the next/previous character in the current line
* `F{char}` Move to the preceding {char}
* Vice versa

## Move horizontally
* `0` Move to the first character of the line
* `^` Move to the first non-blank character of the line
* `$` Move to the last character of the line
* `g_` Move to the last non-blank character of the line

## Page move
* `gg` / `G` Move to the beginning and end of the file
  * `ctrl+o` Quickly return
* `H` /`M` / `L` Jump to the Head, Middle, Lower of screen
* `ctrl+f` / `ctrl+u` Page up
* `ctrl+b` / `ctrl+d` Page down
* `zz` Put the current line in the middle.
