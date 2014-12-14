---
title: Registers
layout: default
---

# Commands

## Number register

- `C-u number C-x r n r`: Insert number into register r.
- `C-u number C-x r + r`: Increment register r by number.
- `C-x r i r`: Insert the number from register r into buffer.


# Examples

List hosts that follow a pattern:

```
C-u 1 C-x r n r
f3
test00 C-x r i r
C-u 1 C-x r + r
RET
f4
C-u 5 C-x e
```
- Insert 1 into register r,
- Start macro recording with `f3`,
- Type beginning of the name of the host, `test00`,
- Insert content of register r at point,
- Increment register r by 1
- Open a new line
- Stop recording macro with `f4`
- Execute macro 5 times.
