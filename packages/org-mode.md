---
layout: default
title: Org-Mode
---

# Visibility

-   `TAB`: Toggle current sub-tree;
-   `S-TAB`: Toggle whole buffer visibility

# Structure Edition

-   `M-RET`: Add new item at the current level;
-   `M-→`: Demote section level.
-   `M-←`: Promote section level.

# Formatting

-   `C-c C-l`: Insert a link.
-   `/italic/`, `*bold*`, `=verbatim=`
-   For enums, use `::` between item header and body.

## Tables

-   Lines beginning with `|` are considered to be part of a table.
-   `TAB`: Reformat table.
-   `C-c -`: (`org-table-insert-hline`) Inserts an horizontal line.
-   `C-c RET`: Insert horizontal line, and go into the row below.
-   `S-M-<left>`: (`org-table-delete-column`) Delete column.
-   `C-c +`: (`org-table-sum`) Sum numbers in the current column, or in
    the rectangle defined by the current region.

See also <http://orgmode.org/manual/Tables.html#Tables> for more
details.

## Links

-   `C-c C-l` to insert a link.
-   `[[ ... ]]` notation can be used to insert any link. The link can be
    internal (use heading text, `#+NAME` property, or add ref
    \`=[]{#ref}=), or external and link to a local file, a URL, a shell
    command etc.

See also <http://orgmode.org/manual/External-links.html>

# Tags

-   `C-c C-t`: Cycles through unmarked, TODO, DONE.
-   `C-c C-c`: Add tag to headline.

# Archiving

-   `C-c $`: Archive current subtree.
-   `C-c a m`: Find all the items that match a rule. `Match:` (e.g.
    `CLOSED<"<-60d>"`, all the DONE items older than 60 days). In the
    Agenda view, items can then be archived using `$`.

# LaTeX Preview

See also <http://orgmode.org/worg/org-tutorials/org-latex-preview.html>

-   `C-c C-x C-l`: LaTeX preview on current line;
-   `C-u C-c C-x C-l`: LaTeX preview on sub-tree;
-   `C-u C-u C-c C-x C-l`: LaTeX preview on the whole buffer;
-   `C-c C-c`: Stop LaTeX preview.

# Example

-   `< e TAB`: Insert example block

# Source code

-   `< s TAB`: Insert source code block
-   `C-c '`: Edit block code in buffer with relevant mode

## Execute code block

Add language to `org-babel-load-languages` (using `customize`), and
execute `C-c C-c`.

# Export

-   `C-c C-e l o`: Export to LaTeX, Compile and open PDF.

Example of a header that can be used:

``` {.example}
#+STARTUP: showall
#+TITLE: Links
#+AUTHOR: Sébastien Le Callonnec
#+LaTeX_CLASS: memoir
#+LaTeX_CLASS_OPTIONS: [a4paper, twoside]
```

A sample header can be added by using `C-c C-e #`.

-   With `org-odt` required, document can be exported to an odt file.

# GitHub Pages

Jekyll uses Markdown, but you can use [Pandoc](https://pandoc.org/) to
convert Org-Mode files to Markdown:

``` {.bash}
pandoc --atx-headers -f org -t markdown org-mode.org -o org-mode.md
```

# Links

-   [org-mode manual](http://orgmode.org/manual/)
-   <http://doc.norang.ca/org-mode.html>
-   [Org Babel code block
    evaluation](https://org-babel.readthedocs.io/en/latest/eval/)
