### Conventions
Here are some common Emacs conventions:

- `C-`: Control key
- `M-`: Meta key; either Alt key or Escape.
- `S-`: Shift key
- `RET` : Return key
- `TAB` : Tab key

For example, when a command is `C-x C-f`, you press `Control` and `x`, and then `Control` and `f`.

### Basic Commands

- `C-x C-f` : Open ("Visit") a file
- `C-x C-v RET` : Reload a file by finding it again.
- `C-x k` : Close file ("Kill buffer")
- `C-x C-s` : Save buffer changes to a file.
- `C-x C-w`: Write file.
- `C-x C-c` : Quit Emacs.

All these key combinations are actually calling Emacs [commands](commands.md).  For example, `C-x C-f` runs the command `find-file`.  The key combination itself is called a [key binding](key-bindings.md).


Next: [Editing](editing.md)