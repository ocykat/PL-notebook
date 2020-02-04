# Vim

## Vimscript

### Cursor

* `line('.')`: current line
* `col('.')`: current column
* `getline('.')`: returns the content of the current line

### Strings

* `strid(a, b)`: if `b` is a substring of `a`, returns the offset of `b` in `a`; else returns `-1`.
* `s[x:y]`: substring of `s` from position `x` to position `y` (inclusively).
* `len(s)`: returns the length of `s`
* `strlen(s)`: similar to `len(s)`

### Some useful functions

```vim
function GetCharUnderCursor()
  return matchstr(getline('.'), '\%' . col('.') . 'c.')
endfunction

function GetSelectedText()
  return getline("'<")[getpos("'<")[2]-1:getpos("'>")[2]]
endfunction

function GetCurrentLine()
  return getline('.')
endfunction

function VisualLength()
  exe 'normal "xy'
  return strlen(@x)
endfunction

function MoveToFirstNonSpace()
  exe 'normal 0'
  if GetCharUnderCursor() == ' '
    exe 'normal w'
  endif
endfunction

function InsertXTimes(str, x)
  exe 'normal ' . string(a:x) . 'a' . a:str
endfunction
```
