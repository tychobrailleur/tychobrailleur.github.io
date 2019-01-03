---
title: Magit
layout: default
---

# Basics

The main entry point of magit is `M-x magit-status`.

Once in the Magit buffer, you can use the following keys:

- `s`: Stage a change
- `c`: Commit
- `k`: Discard a change. Delete a file when untracked.  Delete a
  stash.  Unstage a staged change.
- `l`: log.  `l`, short log, `L` long log
- `+`: enlarge hunk
- `-`: shrink hunk
- `P`: Push
- `F`: Pull

## magit status

In the magit status buffer, you can use `1`, `2`, `3`, `4` to change
the amount of info that can be visualised.

- `C-x C-j`: Jump to file from status to dired.
- `C-c C-e`: On a hunk, jump to file at that change.

# Commits

- `e`: Extend current HEAD coomit
- `a`: Amend the commit message
- `r`: Reword
- `s`: Squash against current commit.

# Magit commands from a file

- `magit-file-popup` : Displays a popup where you can execute magit
  commands on the current file.

# Other Commands

- `magit-push`: Push changes.

# Visualise Log

- `magit-log`: View log for revs input by user.


# User Manual

http://magit.github.io/documentation.html


# Resources

- Magit presentation by John Wiegley https://www.youtube.com/watch?v=j-k-lkilbEs
