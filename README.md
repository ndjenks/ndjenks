- 👋 Hi, I’m @ndjenks
- 👀 I’m interested in electronics and embedded programming
- 🌱 I’m currently learning C, C++, VHDL and Python
- 💞️ I’m looking to collaborate on any interesting projects in safety industrial automation, control systems and motor drives.  
- 📫 How to reach me? Reach me at ndjenkoua@gmail.com

<!---
ndjenks/ndjenks is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

My vim configuration
```
set showmode
set number
set laststatus=2
set relativenumber
set nu rnu

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" " alternatively, pass a path where Vundle should install plugins
" "call vundle#begin('~/some/path/here')
"
" " let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'
"
" " The following are examples of different formats supported.
" " Keep Plugin commands between vundle#begin/end.
" " plugin on GitHub repo
Plugin 'tpope/vim-fugitive'
Plugin 'dense-analysis/ale'
Plugin 'rhysd/vim-clang-format'
Plugin 'puremourning/vimspector'
Plugin 'rust-lang/rust.vim'
Plugin 'Yggdroot/indentLine'
Plugin 'mileszs/ack.vim'
" " All of your Plugins must be added before the following line
call vundle#end()            " required
syntax on
filetype plugin indent on

"Clang format
let g:clang_format#command = "/usr/bin/clang-format"
let g:clang_format#code_style = 'llvm'
let g:clang_format#detect_style_file = 1
let g:clang_format#auto_format_on_insert_leave = 1
autocmd FileType c,cpp ClangFormatAutoEnable

" ALE

"Netrw
let g:netrw_altv=1
let g:netrw_winsize=30
let g:netrw_localrmdir='rm -r'

"Rust
let g:rustfmt_autosave = 1

"indentLine
let g:identLine_color_term = 239
let g:indentLine_char = 'c'
let g:identLine_setColors = 0
let g:indentLine_char_list = ['|', '¦', '┆', '┊']

" Ack
let g:ackprg = 'ag --nogroup --nocolor --column'
```
