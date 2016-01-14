---
title: Version Control
layout: default
---

# Basics

- `C-x v v`: Do the next appropriate VC action.  For example, for git, for a new file, stage the changes.
- `C-x v i`: Stage changes in the current file.
- `C-x v l`: list change log of current fileset.
- `C-x v L`: list change log for the whole tree.
- `C-x v =`: Diff changes
- `C-x v -`: Show old revision in a separate buffer.
- `C-x v g`: blame.


# File Status

The mode line displays details about the file status. For example, for git, it displays `Git-master` when the file is unchanged.  The `-` between `Git` and `master` indicates the status:

- `-`: file is unmodified,
- `:`: file is modified,
- `!`: file contains conflicts,
- `@`: added locally but not yet committed.

# Annotate

Equivalent to _blame_.  Once in `vc-annotate -mode`:

- `j`: Annotate version for the current line.
- `p`: Annotate previous version.
- `n`: Annotate next version.

# Other useful commands

- `vc-region-history`: Gives the history of the region
