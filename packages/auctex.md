---
title: AUCTeX
layout: default
---

This documents AUCTeX and RefTeX.


# Basics

- `C-c C-e`: Add an environment, such as `verbatim`, `itemize`, etc.
- `C-c C-s`: Add sectioning, such as `section`, `subsection`, etc.
- `C-c C-c`: Compile document, or if document is already compile, open
result.
- `C-c C-r`: Partial compiling on region.
- `C-c C-v`: View document.
- `C-c RET`: Add command.
- `C-c ;`: Toggle comments for region.

## Formatting

- `C-c C-f C-i`: Add `textit`.
- `C-c C-f C-b`: Add `textbf`.
- `C-c C-f C-e`: Add `emph`.
- `M-q`: Fill and indent paragraph.
- `C-c C-q C-r`: Fill and indent region.
- `C-c C-q C-s`: Fill and indent section.
- `C-c ~`: Enter math mode.  In math mode, you can enter symbols more
  efficiently by using the ````` prefix.  For example, `\alpha`
  becomes ```a``.

# References

- `C-c =`: (`reftex-toc`) Displays the contents for the current
  document.
- `C-c (`: Inserts a label.
- `C-c )`: Adds a reference to a label.

# Preview

- `C-c C-p C-p`: Preview at point.
- `C-c C-p C-c C-p`: Cancel preview at point.
- `C-c C-p C-r`: Preview region.
- `C-c C-p C-c C-r`: Cancel preview region.
- `C-c C-p C-b`: Preview buffer.
- `C-c C-p C-c C-b`: Cancel preview buffer.

# Link

- Cheat sheet: http://ftp.gnu.org/gnu/auctex/11.86-extra/tex-ref.pdf
- See also [RefTeX](reftex.html)
