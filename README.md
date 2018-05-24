# `math++.el`,
A Mathematica interface for GNU Emacs


Copyright (C) 2009 Daichi Mochihashi <daichi at cslab.kecl.ntt.co.jp>

Installation:

Copy in the `emacs` load path, e.g,

`/usr/share/emacs/site-lis/math++.el`

Add the following lines to your `.emacs` file:

```lisp
(autoload 'math++ "math++" "Starts Mathematica" t)
(autoload 'math-mode "math++" 
    "Mode for editing Mathematica.  Loading will result in more info." t)
(setq auto-mode-alist (cons '("\\.m\\'" . math-mode) auto-mode-alist))
```