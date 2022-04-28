# Vim tips & tricks
## Substitution 
```
:%s/hede/hodo/g
```
###

###
## Syntax highlight
```
:syn on
```
###
###
## Cut/copy/paste/undo/redo
* Cut/Delete char - `x`
* Cut/Delete line - `dd`
* Copy line - `yy`
* Paste - `p`
* Undo - `u`
* Redo - `CTRL-R`
* Repeat last command - `.`
###

###
## Navigate in file
* Go to first line - `:1`
* Go to n'th line - `:n`
* Go to last line - `:$`
* Go to beginning of line  - `^`
* Go to end of line  - `$`
###

###
## Quickly indent/outdent multiple lines

* Enter VISUAL LINE mode by holding [SHIFT] and hitting the “v” key.
* Use the arrow keys or “j” and “k” to select the lines you want to indent.
* Hit the “>” character (hold [SHIFT] and hit the “.” key) to indent.
* Then, you can repeat the indent using the “.” (repeat key) key. Likewise, you can type the “<” character to outdent the selected lines.

###
###
## ~/.vimrc
```
:set guifont=Menlo\ Regular:h16
:colorscheme OceanicNext
if has("gui_macvim")
    let macvim_hig_shift_movement = 1
endif
```
###
