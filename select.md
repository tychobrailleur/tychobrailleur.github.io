---
title: Select
layout: default
---

This page describes how to select text, and introduces the mark, the point and the region.

# Basic

- `C-x h`: `mark-whole-buffer`, select all buffer.

# Mark

To set the mark:

- `C-SPC`: set the mark.  Once the mark is set, you can move your cursor as you want using arrow keys, or even using an incremental search, to adjust your selection.  The current location of the cursor is called the _point_, whilst the actual selected text (between the mark and the point) is called the _region_.
- `C-u C-SPC`: go back to the previous mark.
- `M-@`: set the mark after the end of the next word.
- `M-h`: Mark paragraph
- `C-M-h`: select current function, method, defun in programming.


See [Emacs Manual’s section about the mark](http://www.gnu.org/software/emacs/manual/html_node/emacs/Mark.html#Mark).  Also [“Moving by Defuns”](http://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-by-Defuns.html).

# Narrowing

Narrow means only show a selected part of the buffer, which is very handy to focus on a specific part.

- `C-x n n`: Narrow to the current region.
- `C-x n w`: Widen again.
- `C-x n d`: Narrow to the current function (`defun`)

By default, the narrowing functions are disabled, as they are considered as _confusing_.  When you execute them the first time, you'll be prompted with a message asking you if you want to enable these functions.  You can then choose to permanently enable them.

