---
title: Dired
layout: default
---

In a buffer, use `C-x C-j` to open the current directory in dired.

Once in a dired window (`M-x dired`), the following keys can be used:


## Marking / Unmarking

- `d`: Mark for deletion
- `u`: Unmark for deletion
- `U`: Unmark all
- `* s`: mark all, except for `.` and `..`

## Actions

- `D` : Delete
- `x`: Delete files marked for deletion
- `f` : Visit file
- `o`: Visit file in other window
- `Q`: Query replace on each file marked
- `+`: Create new directory
- `C <name> RET`: Copy with a new name
- `M-x find-grep-dired`: List in a dired buffer files containing
  string matching regexp.


The name of the files can also be edited directly in the dired buffer
by making the buffer writable with `C-x C-q`.
