# My setup
List of Neovim keybindings, snippets, shortcuts and more

## Normal mode
- <leader>w = write/save file
- <leader>q = close file 
- <S-Tab> = shuffle between buffers 
- <S-G> = go to EOF 
- gg = go to BOF 
- i = go insert mode
- 1 = go to the beginning of the line
- 2 = go to the end of the line
- w = shuffle forward by words
- b = shuffle backward by words

## LaTex (vimtex)
- \ll = compile target
- \ls = change target to current .tex
- <Tab> = trigger snippet autocompletion
- <S-Tab> = suffle through snippet insertion points
### Snippets
- ss = superscript
- uu = underscript
- eqref = reference equation
- ref = reference anything
- sys = system of equations
- fdef = map definition
- ex = Example environment
- excont = Continued example
- thm = Theorem environment
- thmcont = Theorem continued
- interp = Interpretation environment
- interpcont = Continued interpretation

## Zotero (zotcite)
- <leader>zi = print title of the ref
- <leader>za = print full details of the ref
- <leader>zo = openf PDF of the ref
- <C-Space> = complete the ref

## File explorer (nvim-tree)
- <leader>e = toggle tree visibility
- <leader>tf = open floating terminal
- i = Open file/folder
