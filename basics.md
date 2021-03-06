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

- `C-x` is called character extend.  It is followed by one character;
- `M-x` is called command extend.  It is followed by a long name.

# Basic Commands

- `C-x C-f` : Open ("Visit") a file
- `C-x C-v RET` : Reload a file by finding it again.
- `C-x k` : Close file ("Kill buffer")
- `C-x C-s` : Save buffer changes to a file.
- `C-x C-w`: Write file.
- `C-x C-c` : Quit Emacs.

All these key combinations are actually calling Emacs
[commands](commands.html).  For example, `C-x C-f` runs the command
`find-file`.  The key combination itself is called a [key
binding](key-bindings.html).

# Navigate

- `C-a`: Go to the beginning of the line.
- `C-e`: Go to the end of the line.
- `C-n`: Next line.
- `C-p`: Previous line.
- `C-l`: `recenter-top-bottom`, move the current line successively to the centre, to the top and then to the bottom of the [window](window.html).
- `M-a`: Go to beginning of sentence.
- `M-e`: Go to end of sentence.
- `M-f`: Move forward by one word.
- `M-b`: Move backward by one word.
- `M-m`: Move to first non-whitespace character of the line (`back-to-indentation`).
- `M-<`: Go to beginning of [buffer](buffer.html).
- `M->`: Go to end of [buffer](buffer.html).
- `M-{`: Go to beginning of paragraph.
- `M-}`: Go to end of paragraph.
- `M-g M-g`: `goto-line`, go to the line number.
- `C-x C-n`: Use the current column as the preferred column when
  moving

# Zooming in/out

- `C-x C--`: Decrease font size (“zoom out”).
- `C-x C-+`: Increase font size (“zoom in”).
- `C-x C-0`: Reset to default size.

# Counting

- `C-x l`: Number of lines in the buffer.
- `M-=`: Number of lines, words and characters in the region.

## In Minibuffer

- `C-M-b`: Go to previous path separator;
- `C-M-f`: Go to next path separator.

Next: [Editing](editing.html)
