***

# Here is my vimrc <img src="https://download.logo.wine/logo/Vim_(text_editor)/Vim_(text_editor)-Logo.wine.png" width="45" height="35" alt=""> 

***

### Absolute essential configurations

***

```vim
syntax on
```
```vim
set noexpandtab
set errorbells
set smarttab
set tabstop=4 softtabstop=4
set shiftwidth=4
set nu
set nowrap
set noswapfile
set incsearch
set number relativenumber
set bg=dark
set encoding=utf-8
set nocompatible
set nohlsearch
set ignorecase
set signcolumn=yes
set scrolloff=8
set colorcolumn=80
set nobackup
set nowritebackup
set cmdheight=2
set updatetime=300
set shortmess+=c
set autoindent
set cindent
set smartindent
```

***

### Here are my plugins:
>I use [vim-plug](https://github.com/junegunn/vim-plug)

***

```vim
call plug#begin()
	Plug 'vim-airline/vim-airline' " looks cool and it's useful
	Plug 'vim-airline/vim-airline-themes'
	Plug 'rafi/awesome-vim-colorschemes' " More colorschemes
    Plug 'neoclide/coc.nvim', {'do': { -> coc#util#install()}} " Autocompletion and much more
    Plug 'junegunn/fzf', { 'do': { -> fzf#install() } } " fzf is a fuzzy finder
    Plug 'junegunn/fzf.vim'
call plug#end()
```

>Plugins:
>* [vim-airline](https://github.com/vim-airline/vim-airline)
>* [rafi-colorschemes](https://github.com/rafi/awesome-vim-colorschemes)
>* [coc.nvim](https://github.com/neoclide/coc.nvim)
>* [fzf.vim](https://github.com/junegunn/fzf.vim)
>for [vim-airline](https://github.com/vim-airline/vim-airline) to work you need to add this setting: `let g:airline_powerline_fonts=1`

***

### Personal settings

```vim
inoremap kj <Esc> "remap kj and jk to escape 
inoremap jk <Esc> "you can remap this to any keys you want
xnoremap K :move '<-2<CR>gv=gv '"(exclude the closing ' ) remap K for moving blocks in visual mode'
xnoremap J :move '>+1<Cr>gv=gv '"(exclude the closing ' ) remap K for moving blocks in visual mode'
nnoremap <silent> :: :Files<CR> "open fuzzy finder faster
```

***
