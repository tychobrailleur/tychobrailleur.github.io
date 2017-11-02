---
title: Org-Mode
layout: default
---

# Visibility

- `TAB`: Toggle current sub-tree;
- `S-TAB`: Toggle whole buffer visibility

# Structure Edition

- `M-RET`: Add new item at the current level;
- `M-→`: Demote section level.
- `M-←`: Promote section level.

# Formatting

- `C-c C-l`: Insert a link.
- `/italic/`, `*bold*`, `=verbatim=`
- For enums, use ` :: ` between item header and body.

## Tables

- Lines beginning with `|` are considered to be part of a table.
- `TAB`: Reformat table.
- `C-c -`: (`org-table-insert-hline`) Inserts an horizontal line.

See also http://orgmode.org/manual/Tables.html#Tables for more details.


## Links

- `C-c C-l` to insert a link.
- `[[ ... ]]` notation can be used to insert any link.  The link can
  be internal (use heading text, `#+NAME` property, or add ref
  ``<<ref>>`), or external and link to a local file, a URL, a shell
  command etc.

See also http://orgmode.org/manual/External-links.html

# Tags

- `C-c C-t`: Cycles through unmarked, TODO, DONE.
- `C-c C-c`: Add tag to headline.


# LaTeX Preview

See also http://orgmode.org/worg/org-tutorials/org-latex-preview.html

- `C-c C-x C-l`: LaTeX preview on current line;
- `C-u C-c C-x C-l`: LaTeX preview on sub-tree;
- `C-u C-u C-c C-x C-l`: LaTeX preview on the whole buffer;
- `C-c C-c`: Stop LaTeX preview.

# Example

- `< e TAB`: Insert example block

# Source code

- `< s TAB`: Insert source code block
- `C-c '`: Edit block code in buffer with relevant mode

## Execute code block

Add language to `org-babel-load-languages` (using `customize`), and
execute `C-c C-c`.

# Export

- `C-c C-e l o`: Export to LaTeX, Compile and open PDF.

Example of a header that can be used:

```
#+STARTUP: showall
#+TITLE: Links
#+AUTHOR: Sébastien Le Callonnec
#+LaTeX_CLASS: memoir
#+LaTeX_CLASS_OPTIONS: [a4paper, twoside]
```

A sample header can be added by using `C-c C-e #`.

- With `org-odt` required, document can be exported to an odt file.

# Links

- [org-mode manual](http://orgmode.org/manual/)
- http://doc.norang.ca/org-mode.html
- [Org Babel code block evaluation](https://org-babel.readthedocs.io/en/latest/eval/)
