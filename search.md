### Search in a buffer

- `C-s` is a forward incremental search
- `C-r` is a backward incremental search

### Search and replace

- `M-%`: `query-replace`
- `C-M-%`: `query-replace-regexp`


### Match Parenthesis

- `C-M-f` : `forward-sexp`, Search matching parenthesis forward
- `C-M-b` : `backward-sexp`, Search match parenthesis backward.

### Search content in files

- `M-x rgrep` : Does a recursive grep.

### Exhuberant Ctags

A tag file must be created with exuberant ctags, for example:

     /usr/local/bin/ctags -e -R -f TAGS --tag-relative

This creates a tag file that will to need to be visited when first searching for a tag.

- `M-.`: search for a tag
- `C-u M-.` : Find next match

