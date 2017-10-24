# Most important Vim commands. A cheat-sheet if you will.
## a set of commands which should be enough to start working smoothly and possible to remember for people whose primary job is to actually code as opposed to geeking with vim and cherishing their .vimrc
## this set is meant to be very short and limited, comprised of commands one should not forget even when "distracted" by work or by particularly ugly pair programmer

### switching modes:
`i` insert, edit before cursor
`a` append, edit after cusor
`shift+a` append at the end of the line
`shift+i` insert at the beginning of the line
`ESC` normal mode

### scrolling:
`zz` move current line to the middle of the screen
`zt` move current line to the top of the screen
`zb` move current line to the bottom of the screen

#### one line
`ctrl+y` move viewport down (somehow doesn't seem to work in IdeaVim)
`ctrl+e` move viewport up (extra lines)

#### half a screen
`ctrl+u` move viewport up
`ctrl+u` move viewport down

### moving around:
`hjkl` don't use these, slow and annoying
`$` end of line
`G$` end of file
`GA` append at eof
`gg` begining of file
`|` or `^` beginning of line (hard/soft)
`12+gg` jump to line number 12
`b` move back one word (B - WORD)
`w` move forward one word (W - WORD)

### selecting:
`v` visual mode
`shift+v` select visual mode by whole lines

### deleting:
`d` delete selected
`dd` delete one line
`d5d` delete 5 lines

### moving fast AND edit at the same time
`bdw` back delete word
`dw` delete from the current cursor position to the beginning of the next word character.
`d$` delete from the cursor position to the end of the line
`d|` or `d^` delete from the cursor to the beginning of the line (hard/soft, means with and without whitespace)
`D` is a synonym for d$.

### surround with vim-surround
`ysiw"` surround word with ""
`ds"` deletes sourrounding ""
`S<b>` surround visual mode selection with closed html or xml tag
`cs"<b>` changes word surrounding "" to <b></b>

### copy paste
`yy` or `Y` yank (copy) the current line
`p` to paste after the cursor
`P` to paste before the cursor
`"3p` pastes the contents of the register 3

### appendix:
- http://vim.wikia.com/wiki/Pasting_registers
- http://vim.wikia.com/wiki/Copy,_cut_and_paste
- https://github.com/tpope/vim-surround -- set surround in your ~/.ideavimrc
- deleting is cutting as well (copy to 'register' or whatever)
- logger.info('last email') is 7 words / 2 WORDS (WORDS are divided by whitespace, words by almost anything)

### saving
`:w`
`:wq`
`:wq!`
