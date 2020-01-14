---
title: CIDER
layout: default
---

See [Manual](https://docs.cider.mx/cider/index.html "Manual") for more
details.

# REPL

- `C-c M-n`: Select a namespace and switch to it.


# Debugging

- `C-u C-M-x`: Instrument an expression.  Expressions can then be
  evaluated using `C-x C-e`.  Once the debugger is started, you can
  use the following keys to use the debugger:
  - `n`: Next expression,
  - `i`: Step into function,
  - `o`: Step out of the current sexp,
  - `c`: Continue,
  - `q`: Quit,
  - `s`: Show the current stack.
