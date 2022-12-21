# ttcn3 mode for Emacs

## Introduction

Here is the original package description written by W. Borgert:

    This is an TTCN-3 editing mode for GNU Emacs (and XEmacs) by me,
    released under the terms of the GNU GPL. It is based on cc-mode,
    the well-known C/C++/IDL/Java/etc. editing mode. This is the world's
    first TTCN-3 editor! The Debian package also contains a very simple
    mode for TTCN (2!), and one for Forth based state machines.

source: https://web.archive.org/web/20121115174612/http://people.debian.org/~debacle/ttcn-free/


## Using

Clone the repo, then add it to the load path and load ttcn3 mode.

The elisp code:

```
(setq ttcn-extension-directory "path/to/directory")

(add-to-list 'load-path ttcn-extension-directory)
(require 'ttcn3)

(autoload 'ttcn3-mode "ttcn3-mode" "TTCN3 editing mode." t)
(setq auto-mode-alist (cons '("\\.ttcn3?" . ttcn3-mode) auto-mode-alist))

```
