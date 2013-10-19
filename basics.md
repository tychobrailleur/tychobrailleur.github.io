---
title: Basics
layout: default
---

# Conventions
Here are some common Emacs conventions:

- `C-`: Control key
- `M-`: Meta key; either Alt key or Escape.
- `S-`: Shift key
- `RET` : Return key
- `TAB` : Tab key

For example, when a command is `C-x C-f`, you press `Control` and `x`, and then `Control` and `f`.

# Basic Commands

- `C-x C-f` : Open ("Visit") a file
- `C-x C-v RET` : Reload a file by finding it again.
- `C-x k` : Close file ("Kill buffer")
- `C-x C-s` : Save buffer changes to a file.
- `C-x C-w`: Write file.
- `C-x C-c` : Quit Emacs.

All these key combinations are actually calling Emacs [commands](commands.html).  For example, `C-x C-f` runs the command `find-file`.  The key combination itself is called a [key binding](key-bindings.html).

# Navigate

- `C-a`: Go to the beginning of the line.
- `C-e`: Go to the end of the line.
- `C-l`: `recenter-top-bottom`, move the current line successively to the centre, to the top and then to the bottom of the [window](window.html).
- `M-<`: Go to beginning of [buffer](buffer.html).
- `M->`: Go to end of [buffer](buffer.html).
- `M-g M-g`: `goto-line`, go to the line number.

Next: [Editing](editing.html)
