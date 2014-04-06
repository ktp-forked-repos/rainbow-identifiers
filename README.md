# Rainbow identifiers mode

Rainbow identifiers mode is an Emacs minor mode providing highlighting
of identifiers based on their names. Each identifier gets a color
based on a hash of its name.

![Screenshot of rainbow identifiers mode on its own code](https://raw.github.com/Fanael/rainbow-identifiers/master/rainbow-identifiers.png)

## Installation

The package is available in [MELPA](http://melpa.milkbox.net/).

If you have MELPA in `package-archives`, use

    M-x package-install RET rainbow-identifiers RET

If you don't, open `rainbow-identifiers.el` in Emacs and call
`package-install-from-buffer`.

## Usage

To toggle the mode

    M-x rainbow-identifiers-mode

To turn it on automatically in most programming modes:

    (add-hook 'prog-mode-hook 'rainbow-identifiers-mode)

## Customization

To change the colors, change faces
`rainbow-identifiers-identifier-<number>`.

To change the number of colors used, change the variable
`rainbow-identifiers-face-count`.
