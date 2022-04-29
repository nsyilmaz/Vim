# Vim tips & tricks
## Substitution 
```vim
:%s/hede/hodo/g
```
#####

## Syntax highlight
```vim
:syn on
```
#####

## Cut/copy/paste/undo/redo
* Cut/Delete char - `x`
* Cut/Delete line - `dd`
* Copy line - `yy`
* Paste - `p`
* Undo - `u`
* Redo - `CTRL-R`
* Repeat last command - `.`
#####

## Navigate in file
* Go to first line - `:1`
* Go to n'th line - `:n`
* Go to last line - `:$`
* Go to beginning of line  - `^`
* Go to end of line  - `$`
#####

## Quickly indent/outdent multiple lines
* Enter VISUAL LINE mode - `SHIFT-V`
* Use the `SHIFT` and `arrow keys` or `j` and `k` to select the lines you want to indent.
* Hit the `>` character (`SHIFT-.`) to indent.
* Likewise, hit the `<` character (`SHIFT-,`) to outdent the selected lines.
* Then, you can repeat the indent using the `.` (repeat key) key. 
#####

## Code completion
* Type something and then press `CTRL-P`
#####

## ~/.vimrc
* Syntax coloring and font settings
```vim
:syn on
:set guifont=Menlo\ Regular:h16
:colorscheme OceanicNext
if has("gui_macvim")
    let macvim_hig_shift_movement = 1
endif
```

* Indentetion and tab settings
```vim
set expandtab       "Use softtabstop spaces instead of tab characters for indentation
set shiftwidth=4    "Indent by 4 spaces when using >>, <<, == etc.
set softtabstop=4   "Indent by 4 spaces when pressing <TAB>
set autoindent      "Keep indentation from previous line
set smartindent     "Automatically inserts indentation in some cases
set cindent         "Like smartindent, but stricter and more customisable
autocmd FileType make set noexpandtab shiftwidth=8 softtabstop=0
```
#####
