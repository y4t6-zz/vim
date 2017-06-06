# vim

`di"` - Удалить текст в кавычках

Нужно пройти `vimtutor`

(можно использовать стрелки для перемещения, но не рекомендуется - их нужно отключить)

[vim-cheat-sheet](http://www.viemu.com/vi-vim-cheat-sheet.gif)

[vimwallpaper](https://i.imgur.com/CjREO9t.png)

[vimgolf](http://vimgolf.com/)

# Конфигурация и плагины

`:set number` - включаем нумерацию строк

`:set expandtab` - устанавливаем пробулы на табы

`:set tabstop=2` - ширина таба в 2 пробела

`vim .vimrc` - создание  .vimrc

```vim
syntax on
colorscheme gruvbox
set background=dark
set number
set expandtab
set tabstop=2

set hlsearch
set incsearch
```

## Поиск по тексту

### Способ 1

`/searching-text` then `Enter`

### Способ 2

`Наводим курсор на слово` then `Нажимаем звездочку`

### Настройка подсветки

`:set hlsearch` - подсвечиваем результаты поиска

`:set incsearch` - инкрементальный поиск

### Доступные плагины

[vundle](https://github.com/VundleVim/Vundle.vim)

[pathogen](https://github.com/tpope/vim-pathogen)

[vimplug](https://github.com/junegunn/vim-plug)

### Конфигурания .vimrc

```vim
" Specify a directory for plugins (for Neovim: ~/.local/share/nvim/plugged)
call plug#begin('~/.vim/plugged')

Plug 'scrooloose/nerdtree', { 'on':  'NERDTreeToggle' }

"colorschemes
Plug 'morhetz/gruvbox'

call plug#end()

"mappings 

map <C-n> :NERDTreeToggle<CR>
```

`:source ~/.vimrc` - вычитываем файл 

`:PlugInstall` - устанавливаем плагин

### Настройка темы

Используем тему [gruvbox](https://github.com/morhetz/gruvbox)
