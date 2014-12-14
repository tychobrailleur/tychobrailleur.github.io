---
layout: default
title: Regexp
---

# Basics

See also https://www.gnu.org/software/emacs/manual/html_node/emacs/Regexp-Replace.html.


- Parentheses for grouping must be escaped.
- Matched group syntax: `\1`, `\2`, etc.
- `\#` counts replacements – first is 0.


# Examples

## Replace comma with newline

`C-q` to escape, and `C-j` to insert newline character.

    M-x replace-regexp RET , RET C-q C-j


## Call elisp function on matched group

Use `\,` before function in the replacement string.

    M-x replace-regexp RET ^"\([a-zA-Z]+\)"$ RET \,(upcase \1)("\1")) RET



