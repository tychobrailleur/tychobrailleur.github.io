---
title: Debugging
layout: default
---

# IELM

- `M-x ielm`: Start interactive emacs lisp


# edebug

- `C-u C-M-x`: `eval-defun` with debug flag.  Start debbuging.
- `M-x edebug-defun`: Start edebug when this function is called.

Once debugger is started:

- `n`: Next step
- `SPC`: Next step
- `e`: Evaluate expression
- `b`: Add breakpoint
- `g`: Execute until next breakpoint
- `o`: Out of the containing sexp – useful in loops
- `q`: Quit debugging
- `r`: Redisplay most recent expression in echo area

# Debugging

- `M-x debug-watch RET <variable> RET` : Watch a variable for any
  change.  When the variable gets set, triggers the debugger and
  displays a stacktrace showing where the variable is being modified.
