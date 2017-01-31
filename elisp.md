---
title: Emacs Lisp
layout:default
---

# Strings

Get text in region:

```
(buffer-substring start end) ;; or buffer-substring-no-properties
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


# Files

```


```


# Buffers

Create a new buffer and switch to it:

```
(with-current-buffer (get-buffer-create "*hi*")
  (pop-to-buffer (current-buffer)))
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
