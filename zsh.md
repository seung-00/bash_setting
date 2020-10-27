## zsh

* Oh my zsh

  ```shell
  $sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  ```

* colorscheme: agnoster

  `$ vim ~/.zshrc`

  ```shell
  ...
  ZSH_THEME="agnoster"
  ```

* plugin

  `$ vim ~/.zshrc`

  ```shell
  ...
  plugins=(
  	git
  	zsh-syntax-highlighting
  	zsh-autosuggestions
  	docker
  	yarn
  )
  ```

* `$ vim ~/.oh-my-zsh/themes/agnoster.zsh-theme`

  ```shell
  prompt_context() {
  	if [[ "$USER" != "$DEFAULT_USER" || -n "$SSH_CLIENT" ]]; then
    	now="$(date +"%H")"
      if [ ${now} -ge 0 -a ${now} -lt 6 ]; then
        emoji="☕️"
      fi
      if [ ${now} -ge 6 -a ${now} -lt 10 ]; then
        emoji="🍳"
      fi
      if [ ${now} -ge 10 -a ${now} -lt 13 ]; then
      emoji="🌳"
     	fi
     	if [ ${now} -ge 13 -a ${now} -lt 17 ]; then
        emoji="🏙 "
  		fi
      if [ ${now} -ge 17 -a ${now} -lt 19 ]; then
       emoji="🌆"
      fi
      if [ ${now} -ge 19 -a ${now} -lt 24 ]; then
       emoji="🌃"
      fi
  
       prompt_segment black default "${emoji}"
    fi
  }
  ```
