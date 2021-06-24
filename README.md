# cursor-flash.el

 * Highlights the cursor on buffer/window-switch

 * Flashes a square of positions around POINT for a customizable
   interval.

 This package temporarily highlights the area immediately
 surrounding POINT when navigating amongst buffers and windows. It
 is intended to assist in visually identifying the current POINT
 and the current window when many windows are on the same frame or
 when windows are very large (related (stackexchange
 question)[https://unix.stackexchange.com/questions/83167/emacs-finding-the-cursor-in-multiple-windows]).

## Dependencies: NONE

## Installation:

   1) Evaluate or load or install this file.

   2) Optionally, define a global keybinding or defalias for function
      `cursor-flash-mode`
```
         (global-set-key (kbd "foo") 'cursor-flash-mode))
         (defalias 'cursor-flash-mode 'foo)
```

   3) Optionally, To automatically enable the mode when starting Emacs, add an
      equivalent of the following to your init file:
```
         (require 'cursor-flash)
         (cursor-flash-mode 1)
```

## Operation:

   M-x `cursor-flash-mode`

## Configuration:

   M-x `customize-group` <RET> cursor-flash <RET>

   You can customize variable `cursor-flash-interval` and face
   `cursor-flash-face`.

## Compatibility:

  * Tested on Debian Emacs 27 nox.

  * Includes support to operate nicely with `yascroll-bar-mode` and
    `vline-mode`. It temporarily suspends those modes locally
    during a flash in order not to make the buffer display jump
    around.

## Feedback:

  * It's best to contact me by opening an 'issue' on the package's
    github repository or, distant second-best, by direct e-mail.

  * Code contributions are welcome and github starring is appreciated.

## Colophon:

* Copyright (C) 2021 Boruch Baum <boruch-baum@gmx.com>
* Author/Maintainer:  Boruch Baum <boruch-baum@gmx.com>
* Homepage: https://github.com/Boruch-Baum/emacs-cursor-flash
* License: GPL3+

## Some other Emacs software that I've published

* Diredc [![MELPA](https://melpa.org/packages/diredc-badge.svg)](https://melpa.org/#/diredc) [![MELPA Stable](https://stable.melpa.org/packages/diredc-badge.svg)](https://stable.melpa.org/#/diredc)
  * Large collection of interoperable dired extensions
  * https://github.com/Boruch-Baum/emacs-diredc

* Crossword
  [![MELPA](https://melpa.org/packages/crossword-badge.svg)](https://melpa.org/#/crossword)
  [![MELPA Stable](https://stable.melpa.org/packages/crossword-badge.svg)](https://stable.melpa.org/#/crossword)
  * Download and play crossword puzzles, in Emacs!
  * https://github.com/Boruch-Baum/emacs-crossword

* Emacs-w3m
  * Extensions to the classic web browser (fork)
    * Advanced downloader (bulk, regex, queue management, resume aborted)
    * Scrub history
    * More ...
  * https://github.com/Boruch-Baum/emacs-w3m

* Key-assist
  [![MELPA](https://melpa.org/packages/key-assist-badge.svg)](https://melpa.org/#/key-assist)
  [![MELPA Stable](https://stable.melpa.org/packages/key-assist-badge.svg)](https://stable.melpa.org/#/key-assist)
  * Simple keybinding cheatsheet and launcher
  * https://github.com/Boruch-Baum/emacs-key-assist

* xhair
  * Highlight the current line and column
  * https://github.com/Boruch-Baum/emacs-xhair

* Home-end
  [![MELPA](https://melpa.org/packages/home-end-badge.svg)](https://melpa.org/#/home-end)
  [![MELPA Stable](https://stable.melpa.org/packages/home-end-badge.svg)](https://stable.melpa.org/#/home-end)
  * Turn home and end keys to multi-use navigation keys
  * https://github.com/Boruch-Baum/emacs-home-end

* Keypress-multi-event
  [![MELPA](https://melpa.org/packages/keypress-multi-event-badge.svg)](https://melpa.org/#/keypress-multi-event)
  [![MELPA Stable](https://stable.melpa.org/packages/keypress-multi-event-badge.svg)](https://stable.melpa.org/#/keypress-multi-event)
  * perform different actions when repeating a key
  * https://github.com/Boruch-Baum/emacs-keypress-multi-event

* Post-mode  - Updates to the abandoned email editing package (fork)
  * https://github.com/Boruch-Baum/post-mode
