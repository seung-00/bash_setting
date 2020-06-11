# my bash setting

## vim

* plugin manager: vundle

  ```sh
  $git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  ```

* dracular

  ```shell
  :PluginInstall
  ```

* suntax on, line numbering, c indent


## zsh

* Oh my zsh

  ```shell
  $sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  ```

* dracular

  ```shell
  $git clone https://github.com/dracula/zsh.git
  $cp zsh/dracula.zsh-theme /Users/{Username}/.oh-my-zsh/themes/dracula.zsh-theme
  $cp -r zsh/lib /Users/{Username}/.oh-my-zsh/themes/lib
  ```

  ```shell
  $vim ~/.zshrc
  ...
  ZSH_THEME="dracula"
  ```

* plugin

  ```shell
  $vim ~/.zshrc
  ...
  plugins=(
    git
    zsh-syntax-highlighting
    zsh-autosuggestions
  )
  ```

  

## iterm2

* dracular

  ```shell
  $ git clone https://github.com/dracula/iterm.git
  ```

* Preferences
  * Apperance -> General -> Theme: Dark
  * Apperance -> window -> check "Hide scrollbars"
  * Apperance -> window -> uncheck "Show line under title bar when the tab bar is not visible"

