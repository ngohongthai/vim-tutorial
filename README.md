# vim-tutorial
### note
- Add new file: vim filename.txt
- Save and Quit: ESC + :wq
- on/off ruler: set ruler!
- zz of Z: change the view to the center
### Navigations commands:
- Move up: k
- Move down: j
- M:ove right: l
- Move left: h
- Page down: ctrl + f
- Page up: ctrl + b
- move forward by word: w
- move backward by word: b
- to move to the top file: gg or 1gg
- to move to the last line: $G or just G (shift + g)
- To go to a specific line number: :[number][Enter] or [number]gg
- To move to the end of the line: $ (shift + 4)
- To move to the head line: 0
### Deleting Text
- delete character: move cursor to the character and press x
- delete word: use "w" to move to the word need to be deleted and press: dw
- d + (h-left,j-down,k-up,l-right)
  + dh: delete the left character
  + dl: delete current charater
  + dk: delete current line and above line
  + dj: delete current line and below line
  + dd: delete current line
- d + ($- end line, 0 - head line)
  + d$: delete from cursor to the end of the line
  + d0: delete from cursor to the head of the line

note
- [number] + command : [number] time to repeat the command
- open help in: help.txt

### Cut, Copy and Paste
- dd: cut line
- p: paste
- y: copy line
- yw: copy word
- u: undo
- ctrl + r: redo

