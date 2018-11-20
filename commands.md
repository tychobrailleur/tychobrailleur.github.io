---
title: Commands
layout: default
---

A command is an interactive function, i.e. a function that can be
called using `M-x`, or bound to a key sequence.

- `C-x` is called character extend.  It is followed by one character;
- `M-x` is called command extend.  It is followed by a long name.

# Cancelling

- `C-g`: cancel command.
- `ESC ESC ESC`: either quit or abort.

# Repeating

- `C-x z`: Repeat previous command.
- `C-x z z z`: Repeat previous command three times.
- `M-x repeat-complex-command`: Edit and re-evaluate the last complex
  command, i.e. the last one that used the minibuffer.

# More

`C-x` uses a keymap where the bindings are defined.  This keymap is stored in
`ctl-x-map`.  To see this map, just use `C-h v ctl-x-map`.  See
[help](help.html) for more details on Help commands.

# Minibuffer

Change `history-length` variable to incrase history size.  Default is 30.

- `C-M-b`: Go to previous path separator;
- `C-M-f`: Go to next path separator.
- `M-p`: Also up arrow. Previous command in history.
- `M-n`: Also down arrow.  Next command in history.
- `C-r`: Search back in command in history
- `M-x list-command-history`: List commands in history.  Use `x` to
  execute one of the commands in the list.
