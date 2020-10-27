## vimrc

* `~/.vimrc`

* plugin manager: vundle

  ```sh
  $git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  ```

* colorscheme: dracular

* Plugins

  ```shell
  1 set rtp+=~/.vim/bundle/Vundle.vim
  2 call vundle#begin()
  3 Plugin 'VundleVim/Vundle.vim'
  4 Plugin 'preservim/nerdtree'
  5 Plugin 'nathanaelkane/vim-indent-guides'
  6 Plugin 'terryma/vim-multiple-cursors'
  7 Plugin 'Dracula/vim'
  8 Plugin 'isRuslan/vim-es6'
  9 Plugin 'pangloss/vim-javascript'
  10 Plugin 'mxw/vim-jsx'
  11
  12 call vundle#end()            " required
  13 filetype plugin indent on    " required
  14
  15 syntax on
  16 set number
  17 set autoindent " 자동 들여쓰기
  18 map <Enter> o<ESC>
  19 colorscheme dracula
  20
  21
  22 "Nerd Tree"
  23 map nerd :NERDTreeToggle<CR>
  24 map <C-t>  :tabnew<CR>
  25 nmap <C-H> <C-W>h
  26 nmap <C-J> <C-W>j
  27 nmap <C-K> <C-W>k
  28 nmap <C-L> <C-W>l
  29
  30 "Multiple Cursors
  31 map <C-d> <C-n>
  32 "
  33 map <silent> <C-o> :NERDTreeToggle<CR>
  ```

  * syntax on, line numbering, c indent

  * Shortcut

    * Multiple Cursors
      * `ctrl + d`
    * Nerd Tree
      * nerdtree with toggle: `nerd`
      * new tab: `ctrl + t`
      * cursor move: `ctrl + h,j,k,l`
      * Install: `:PluginInstall`

  * install: `:PluginInstall`

    