---
title: Emacs Lisp
layout: default
---
# Numbers

Largest value for a Lisp integer: `most-positive-fixnum`


# Strings

Get text in region:

```
(buffer-substring start end) ;; or buffer-substring-no-properties
```

Replace regexp `substr` with `replace-str` in string `str`:

```
(replace-regexp-in-string substr replace-str str t t)
```


# Lists

Remove odd numbers:

```
(remove-if-not #'(lambda (x) (zerop (mod x 2))) (number-sequence 1 10))
```

Sum all even numbers below 10:

```
(apply '+ (remove-if-not #'(lambda (x) (zerop (mod x 2))) (number-sequence 1 10)))
```

Apply function to a list:

```
(mapcar (lambda (e) (upcase e)) '("one" "two" "three"))
```

# Files

Write a string `str` to a file `file-path`

```
(write-region str nil file-path nil nil nil t)
```


# Buffers

Create a new buffer and switch to it:

```
(with-current-buffer (get-buffer-create "*hi*")
  (pop-to-buffer (current-buffer)))
```

# Run Commands

Run command `cmd`, save into a string, and append to buffer `buffer`:

```
(with-current-buffer buffer
      (goto-char (point-max))
      (insert (shell-command-to-string cmd)))
```

# Common Lisp

## For Loop

```
(defun fizzbuzzp (n)
  (or (zerop (mod n 3)) (zerop (mod n 5))))
(loop for i from 1 to 999 when (fizzbuzzp i) summing i)
```

### Nested Loop

```
(loop with product = '()
      for i from 1 to 10
      do (loop for j from 1 to 10 do (push (* i j) product))
      finally return (nreverse product))
```



# Misc

Automatically add GNU headers in Elisp file: `M-x auto-insert`


# Elisp REPL

```
M-x ielm
```
