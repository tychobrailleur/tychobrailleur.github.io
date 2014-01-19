---
title: Commands
layout: default
---

A command is an interactive function, i.e. a function that can be called using `M-x`, or bound to a key sequence.

- `C-x` is called character extend.  It is followed by one character;
- `M-x` is called command extend.  It is followed by a long name.

# Cancelling 

- `C-g`: cancel command.
- `ESC ESC ESC`: either quit or abort.

# Repeating

- `C-x z`: Repeat previous command.
- `C-x z z z`: Repeat previous command three times.

# More

`C-x` uses a keymap where the bindings are defined.  This keymap is stored in
`ctl-x-map`.  To see this map, just use `C-h v ctl-x-map`.  See
[help](help.html) for more details on Help commands. 
