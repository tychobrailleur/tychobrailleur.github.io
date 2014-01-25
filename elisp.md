---
title: Emacs Lisp
layout:default
---

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
