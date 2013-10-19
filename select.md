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

See [Emacs Manual](http://www.gnu.org/software/emacs/manual/html_node/emacs/Mark.html#Mark)

# Narrowing