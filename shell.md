---
title: Shell
layout: default
---

# Execute External Commands

- `M-!` : `shell-command`, execute entered command and insert output in minibuffer.
- `C-u M-!` : execute command and insert output at point.
- `M-|`: `shell-command-on-region`, executes command using region as input.
- `C-u M-|`: same, but replaces region with output from command.

   Example:

   ```
   C-u M-| uniq
   ```

# Shell

A shell session can be started with `M-x shell`

# EShell

EShell is the Emacs shell
