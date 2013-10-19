---
title: Buffers
layout: default
---

# Basics

- `C-x b blah` : Reopen `blah` buffer
- `C-x C-b`: List all the buffers
- `M-x eval-buffer`: Eval buffer. Useful to reload `.emacs` after having modified it.
- `C-x C-q`: Toggle read-only.

# Ibuffer

To use Ibuffer when listing all the buffers, add the following to your `init` file: 

    (defalias 'list-buffers 'ibuffer)