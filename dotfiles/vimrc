set nocompatible
set hlsearch
set incsearch
set ignorecase
set smartcase
set number
set backspace=2
set nowrap
set nofixeol
set noswapfile
set history=1000
set autoread
set ic
set ruler
set hidden
colo delek
syntax on
let c_no_curly_error = 1

" -- IDENT
filetype plugin indent on
set smarttab
set smartindent
set autoindent
set tabstop=4
set shiftwidth=4
set expandtab
set list listchars=tab:\ \ ,trail:·

" -- UNDO
set undofile
set undodir=$HOME/.vim/backup
set undolevels=1000
set undoreload=10000
if has("autocmd")
  au BufReadPost * if line("'\"") > 1 && line("'\"") <= line("$") | exe "normal! g'\"" | endif
endif

" -- TAGS
set autochdir
set tags=tags;
noremap <c-n> <c-w>g<c-]>
noremap <c-b> <c-t>

" -- TABS
set tabpagemax=128
map <c-h> gT
map <c-l> gt
set tabline=
set winminwidth=0
map <c-j> <c-w>j<c-w>_
map <c-k> <c-w>k<c-w>_

" -- TABS
set scrolloff=8
set sidescrolloff=15
set sidescroll=1
