# go.vim

An attempt to bring full featured Go support to Vim. All necessary binaries are
installed once at startup (can be disabled if path is provided, see
[#Customize]()).


## Features

* Syntax highlighting
* Auto go fmt on save
* Autocomplete with `<C-x><C-o>` (omnicomplete)

## Install

If you use pathogen, just clone it into your bundle directory:

```bash
$ cd ~/.vim/bundle
$ git clone git://github.com/fatih/go.vim.git
```

Autocompletion is enabled by default via `<C-x><C-o>`, to get real-time
completion (completion by type) install YCM:

```bash
$ cd ~/.vim/bundle
$ git clone git@github.com:Valloric/YouCompleteMe.git
$ cd YouCompleteMe
$ ./install.sh
```

## Customize

```vimrc
" disable auto go fmt on save
let g:go_fmt_autosave=0

" change gocode path, disables automatic installing of gocode
let g:gocode_bin="~/custom/path"

```
