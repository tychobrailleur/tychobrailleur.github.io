---
title: Search
layout: default
---

This page covers:

- Searching for text in buffers and files;
- Searching for files whose name matches certain patterns.

# Search in a buffer

- `C-s` is a forward incremental search
- `C-r` is a backward incremental search

## Ibuffer

In Ibuffer, you can select buffers to do an incremental search on them.  To mark buffers in the list, press `m`.

Then:

- `M-s a C-s`: Incremental search on marked buffers.  When the end of a buffer is reached (with `C-s`, it goes to the next marked one.  Once all the buffers have been searched, it rotates back to the first buffer.
- `M-s a C-M-s`: Isearch for regexp in the marked buffers.

# Search and replace

- `M-%`: `query-replace`
- `C-M-%`: `query-replace-regexp`


# Match Parenthesis

- `C-M-f` : `forward-sexp`, Search matching parenthesis forward
- `C-M-b` : `backward-sexp`, Search match parenthesis backward.

# Search content in files

- `M-x rgrep` : Does a recursive grep.

# Exhuberant Ctags

A tag file must be created with exuberant ctags, for example:

     /usr/local/bin/ctags -e -R -f TAGS --tag-relative

This creates a tag file that will to need to be visited when first searching for a tag.

- `M-.`: search for a tag
- `C-u M-.` : Find next match

