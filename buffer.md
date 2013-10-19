---
title: Buffers
layout: default
---

# Basics

- `C-x b blah` : Reopen `blah` buffer.  With [Ido](packages/ido.html), the minibuffer suggests a list of possible buffers.
- `C-x C-b`: List all the buffers.  See Ibuffer for improvements.
- `M-x eval-buffer`: Eval buffer. Useful to reload `.emacs` after having modified it.
- `C-x C-q`: Toggle read-only.

# Ibuffer

Ibuffer is a mode that lets you manage buffers in a very similar way that [Dired](packages/dired.html) lets you manage files.

To use Ibuffer when listing all the buffers, add the following to your `init` file: 

    (defalias 'list-buffers 'ibuffer)