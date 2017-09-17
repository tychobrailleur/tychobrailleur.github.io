---
title: Dired
layout: default
---

In a buffer, use `C-x C-j` to open the current directory in dired.

Once in a dired window (`M-x dired`), the following keys can be used:


## Marking / Unmarking

- `d`: Mark for deletion
- `t`: Mark all
- `u`: Unmark for deletion
- `U`: Unmark all
- `* s`: mark all, except for `.` and `..`
- `* .`: mark all files with a given extension
- `* %`: mark all files matching a given regexp

## Actions

- `D` : Delete
- `x`: Delete files marked for deletion
- `f` : Visit file
- `o`: Visit file in other window
- `Q`: Query replace on each file marked
- `+`: Create new directory
- `C <name> RET`: Copy with a new name
- `w`: Copy name of file under cursor (or selected) into kill-ring
- `0 w`: Copy absolute path of file
- `! cmd RET`: Execute command `cmd` on file.
- `M-x find-grep-dired`: List in a dired buffer files containing
  string matching regexp.
- `M-x find-dired`: Find and list in a dired buffer files matching
  find command.


The name of the files can also be edited directly in the dired buffer
by making the buffer writable with `C-x C-q`.


## Example

To search and replace in a given folder:

- Search for all occurrences in a given folder, using `M-x
  find-grep-dired`
- Mark all the buffers by using `t` in dired.
- Press `Q` to start query-replace on the marked buffers.
- You can use `!` to get all the occurrences in a buffer replaced.
- You can then use `C-x s` to save all the buffers.
