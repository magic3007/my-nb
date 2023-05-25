# Shortcuts

#cheatsheet

This cheatsheet summarizes the most frequently used shortcuts in my daily routine. 
Some shortcuts are defined as the manual, and  others are custom. The cheatsheet is 
arranged by the workspace.

## iterm2 

```bash
#  * shortcuts in GNU readline
# Reference:
# - https://www.masteringemacs.org/article/keyboard-shortcuts-every-command-line-hacker-should-know-about-gnu-readline

Ctrl-b        # move backward one character
Ctrl-f        # move forward one character

Alt-b         # move backward one word
Alt-f         # move forward on word

Ctrl-a        # move to the begin of the line
Ctrl-e        # move to the end of the line

Ctrl-d        # delete character forward
backspace     # delete character backward

Ctrl-w        # kill word forward
Alt-d         # kill word backward

Ctrl-k        # kill (to clipboard) to the end of line
Ctrl-u        # kill (to clipboard) to the beginning of line

# delete: only delete word
# kill:   delete word and save to clipboard
# Note: Although GNU readline maintains a kill ring (clipboard), works much like
# Emacs’s kill ring, it’s not shared with your system’s clipboard, nor any other
# instances of GNU readline.  It is, in effect, local to the process you’re
# running.

Ctrl-y                  # yank from kill ring
Alt-y                   # (after Ctrl-y) cycle through kin ring history

Alt-t         # swap word
Ctrl-t        # swap character

Alt-u         # Upper forward word
Alt-l         # Lower forward word
Alu-c         # Capitalize forward word

Ctrl-/ 
Ctrl--        # Cycle through the undo list

# * shortcuts in neovim

<Space>-tk     # telescope keymaps
<Space>-lf     # format files

# * shortcuts in gdb dashboard

# To change the layout, e.g., show only source, expressions, and disable assembly, run:
dashboard -layout source expressions !assembly
```

## Vscode for MacOS
```bash
Shift-Command-E # show explores / troggle focus
Command-\       # split editor


```
## Chrome

```bash
Ctrl-l        # focus on the address bar 
<Esc>         # focus from the address bar to the page
```

## MacOS  

```bash

# * shortcuts provided by Rectangle
Ctrl-Option-Cmd-<left/right arrow>               # move the current window the left/right screen 
Ctrl-Option-<left/right/up/down arrow>           # move left/right/top/bottom half

```
