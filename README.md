# Grand Shell Emacs Theme #

Dark color theme for Emacs >= 24 with intensive colors suited to my taste :)

![screenshot](https://raw.github.com/steckerhalter/grandshell-theme/master/grandshell-theme.png)

## Installation ##

### quelpa

`quelpa` is at https://github.com/quelpa/quelpa

```lisp
(quelpa '(grandshell-theme :repo "steckerhalter/grandshell-theme" :fetcher github))
;; since the recipe is stored in melpa this also works:
(quelpa 'grandshell-theme)
```
Interactively: `M-x quelpa grandshell-theme RET`.

### melpa

You can install the theme using the packages on [melpa](https://melpa.org/) (see there for instructions how to set it up).

Then use `M-x package-list-packages`, select `grandshell-theme` from
the list by pressing `i`, then press `x` to execute the changes.

### el-get

Here's a basic recipe you can use to install it via el-get:

    (:name grandshell
           :type github
           :pkgname "steckerhalter/grandshell-theme"
           :minimum-emacs-version 24
           :post-init (add-to-list 'custom-theme-load-path default-directory))

## Usage

In Emacs24 you can just use `M-x customize-themes` to select themes.

If you want to load the theme in your `.emacs` or similar you can add:

    (load-theme 'grandshell t)

and the theme should be loaded and activated on startup.
