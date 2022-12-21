# ttcn3 mode for Emacs

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
