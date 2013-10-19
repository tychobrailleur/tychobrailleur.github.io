### New File

A new file can be created in two ways:
- Open a non-existing file from the command line with emacs: `$ emacs my_new_file`.  This will open a new empty buffer.
- Create a new buffer in Emacs by typing `C-x b` name of the buffer `RET`.  This creates a new buffer you can edit.  You can then [save to a file](editing.md#save).

### Save

Use `C-x C-s` to save a buffer changes to a file.  If there is no file associated to a buffer, the minibuffer will prompt for one.

### Copy-Paste 

Copy-paste is easier to do with CUA mode active.  To activate CUA mode, go to the _Options_ menu and make sure _Use CUA Keys_ is ticked.  To save, _Options_ → _Save Options_.  Another way of activiating it is by adding the following to your [`init` file](init-file.md):

    (cua-mode t)

Once CUA mode is active, copy-paste functions are bound to the usual keys:

- `C-c`: Copy
- `C-p`: Paste
- `C-x`: Cut


### Undo-Redo

- `C-_` : undo
- `C-g C-_` : Redo after undo
- `C-g C-/` : Redo after undo

When CUA mode is active, `C-z` also acts as undo.

See also http://www.gnu.org/software/emacs/manual/html_node/emacs/Undo.html

### Formatting

- `M-c` : capitalize word
- `M-u` : uppercase word
- `M-l` : lowercase word
- `M-x center-line` : center the text on the line.

Next: [Search](search.md)