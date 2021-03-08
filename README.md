# dotfiles

## My dotfiles.

- .vimrc
- ~~.vscode/settings.json~~
  - **This file is no more managed**

## Usage

### neovim

```sh
$ sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'

$ mkdir ~/.config/nvim
$ cd ~/.config/nvim
$ ln -sf ~/gitFolders/dotfiles/.vim/vimrc init.vim
$ vim init.vim

# Run :PlugInstall
```

### vim

```sh
$ curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
$ cd .vim
$ ln -sf ~/gitFolders/dotfiles/.vim/vimrc vimrc
$ vim vimrc

# Run :PlugInstall
```

### tmux

```sh
$ cd ~
$ ln -sf ~/gitFolders/dotfiles/.tmux.conf .tmux.conf
```
