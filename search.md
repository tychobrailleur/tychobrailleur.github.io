---
title: Search
layout: default
---

This page covers:

- Searching for text in buffers and files;
- Searching for files whose name matches certain patterns.

# Search in a buffer

- `C-s` is a forward incremental search.  `M-%` to replace found occurrence.
- `C-r` is a backward incremental search
- `M-x list-matching-lines`: list lines matching a regexp in the
  current buffer.

In search mode, the following bindings are available:

- `M-e`: Edit search string
- `M-s c`: Toggle case-sensitive search
- `M-s o`: List occurrences of search string

## Search in multiple buffers

- `M-x multi-occur-in-matching-buffers RET .* RET <text> RET`: Search
  in all open buffers.

## Ibuffer

In Ibuffer, you can select buffers to do an incremental search on them.  To mark buffers in the list, press `m`.

Then:

- `M-s a C-s`: Incremental search on marked buffers.  When the end of
  a buffer is reached (with `C-s`, it goes to the next marked one.
  Once all the buffers have been searched, it rotates back to the
  first buffer.
- `M-s a C-M-s`: Isearch for regexp in the marked buffers.

# Search and replace

- `M-%`: `query-replace`
- `C-M-%`: `query-replace-regexp`

## Search and Replace in several files

- `M-x find-name-dired t Q`: Prompts for interactive query-replace in files
  selected in dired.  Use `y` to accept replace. `C-x s !` to save
  all.

## Search and Replace with across multiline regions

Newlines must be entered using `C-q C-j`.  For example, to remove
trailing commas in a JSON file, the regexp should be:

```
,\([
 ]+},\)
```

the newline being inserted with `C-q C-j`.

## Examples

- Remove `^M` characters:

```
M-% C-q C-M RET RET
```

## Replace with a Lisp expression

```
 M-x replace-regexp <RET> ^.\{0,72\}$ <RET>
         \,(format "%-72sABC%05d" \& \#) <RET>
```

- `\&` : Represents the whole match being replaced
- `\#` : Count of replacement so far, starting with 0
- `\1`, `\2`, ...: Grouped match.
- `\#1`, `\#2`, ...: Grouped match as a number.

# Match Parenthesis

- `C-M-f` : `forward-sexp`, Search matching parenthesis forward
- `C-M-b` : `backward-sexp`, Search match parenthesis backward.

# Search content in files

- `M-x rgrep` : Does a recursive grep.
- To navigate in `grep-mode`:
- `}`, `TAB`: Next match
- `<`: Beginning of buffer
- `>`: End of the buffer.

# Exhuberant Ctags

A tag file must be created with exuberant ctags, for example:

     /usr/local/bin/ctags -e -R -f TAGS --tag-relative

This creates a tag file that will to need to be visited when first searching for a tag.

- `M-.`: search for a tag
- `C-u M-.` : Find next match
- `M-*` : `pop-tag-mark`, Go back to previous location

# Highlighting

- `C-x w h <regexp> RET <face> RET` : Highlight regexp.  To then deactivate highlighting, `C-x
  w r`.
- `C-x w l <regexp> RET <face> RET`: Highlight lines containing regexp.

# Misc Commands

- `M-x cd`: Change default directory.  Often needed when using search
  commands that operate from current directory.


# Find a file

  - `find-name-dired`: Searches file pattern in a given base directory
  - `locate`: Searches file using a search string.


Next: [Select](select.html)
