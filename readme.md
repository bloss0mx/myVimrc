# readme

## 特性

主要用于前端开发，使用一些基本插件，诸如高亮，自动提示，lint

平台：Mac

## 系统准备

### bat

> https://github.com/sharkdp/bat

sharkdp/bat 替代 cat 并实现语法高亮

安装：

```bash
brew install bat
```

### fzf

> https://github.com/junegunn/fzf

junegunn/fzf

超快文件搜索，同时可以预览文件

安装：

```bash
brew install fzf
```

### ag

> https://github.com/ggreer/the_silver_searcher

ggreer/the_silver_searcher 替代 vimgrep 实现文本搜索，会自动忽略.gitignore 里的文件

### fd

> https://github.com/sharkdp/fd

sharkdp/fd 文件搜索器

安装：

```bash
brew install fd
```

### bashrc/zshrc

```plain
export FZF_DEFAULT_COMMAND='fd --type f'
export FZF_CTRL_T_COMMAND="$FZF_DEFAULT_COMMAND"
```

## vim 包管理工具

### vundle

> https://github.com/VundleVim/Vundle.vim

使用 VundleVim/Vundle.vim 进行插件管理。

安装：

```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

### vim-plug

使用 junegunn/vim-plug 来管理余下的插件
（其实这里是以前瞎搞留下的问题，以后看看能不能统一用 vundle）

安装：

```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

### coc.nvim

使用的 coc 插件：

1. coc-css
1. coc-emmet
1. coc-eslint
1. coc-git
1. coc-highlight
1. coc-json
1. coc-markdownlint
1. coc-pairs
1. coc-prettier
1. coc-tabnine
1. coc-tsserver

## 主要插件的使用方法

使用`:`开始输入指令

- 文件目录 NERDTreee
- 文件搜索 Files
- 文本查找 Ag

## TODO

考虑提供一个脚本直接安装本 vimrc
