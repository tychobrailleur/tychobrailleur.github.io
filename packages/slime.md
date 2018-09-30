Install Slime
=============

Install quicklisp
=================

Install clhs
============

<https://github.com/Hexstream/clhs>

In Slime:

    (ql:quickload "clhs")
    (clhs:print-emacs-setup-form)

Then in your init file:

``` {.commonlisp}
(load "~/quicklisp/clhs-use-local.el" t)
```
