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
- delete word: use "W" to move to the word need to be deleted and press: dW
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
- shift + p : paste above line
- y: copy line
- yw: copy word
- u: undo
- ctrl + r: redo
### Register
- "[register name][command]
   - e.g:
	 + "ayy -> copy line and save named a
	 + "ap -> paste above copy 
- list available register: :registers

### Inserting, Changing, Replacing and Joining
- A (shift + a): Insert at the end of line
- o : Insert a line below
- O (shift + o): Insert a line above
- If you want to insert 80 asterisks characters: 80 + i (for insert mode) + * + ESC
- Create 5 lines that begin with "#": 5 + o + # + ESC
- R or shift + r : Replace
- guu : change the current LINE from upper to lower
- gUU: change the current LINE from lower to upper
- guw: change to end of current WORD from upper to lower
- guaw: change all current WORD to lower
- gUw: change to the end of current WORD to upper
- gUaw: change all current WORD to upper

- shift + ~ : change one character to upper/lower
- g~~ : Invert case to entire LINE
- g~w: Invert case to current WORD
- guG: Change to lowercase until the end of document.

- J (shift + j): Combine two line (Vim will add space)
- gJ : Combine two line without adding a space

### Searching, Search and Replace
- /text : search text (Search in forward direction), ?text: Search in backward direction
- n: find next occurrence
- N: find previous occurrence
- //: Repeat previous foward search
- * : Search word under cursor (next) 
- # : Search word under cursor (previous)
- :vimgrep searchText filename.txt or * .txt
   + :cn : find next
   + :cN : find previous

