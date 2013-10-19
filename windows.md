---
title: Windows and Frames
layout: default
---

Windows are different portions visible within the same UI “window”, whereas frames are actually separate UI “windows.”

# Split Window

- `C-x 2`: Split the current window into two windows, one above the other (`split-winbdow-vertically`).
- `C-x 3`: Split the current window into two windows, side by side (`split-windows-horizontally`)
- `C-x o`: Go into the next window.
- `C-x 0`: Delete the current window.
- `C-x 1`: Close all the windows, except for the current one.
- `C-x }`: Shrink window (`C-u C-x }` shrinks 4 times, `C-u C-u C-x }` 16 times, etc.)
- `C-x {`: Increase window size

# Frame

- `C-x 5 2` : Create new frame.
- `C-x 5 o`: Go into the other frame.
- `C-x 5 0`: Delete the current frame.
- `C-x 5 1`: Delete all the frames, except for the current one/

# Menus and Toolbars

To permanently hide the menubar and the toolbar, add the following to your `init` file:

   (menu-bar-mode nil)
   (tool-bar-mode nil)