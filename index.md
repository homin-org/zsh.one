---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---

# install ohmyzsh plugins
> in an esay way

1 click script

```sh <(curl -L get.zsh.one)```

> or in a hard way

- install zsh first

```sudo apt update && sudo apt install -y zsh```

- install requirements

```sudo apt install -y curl git vim nano```

- install ohmyzhs

```sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

- zsh-autosuggestions

```git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions```

- zsh-syntax-highlighting

```git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting```

- zsh-completions

``` git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions```

- make .zshrc backup and edit .zshrc

```cp .zshrc .zshrc.bak```

```vim .zshrc```

- find ```plugins=(git)``` line

type ```dd``` to delete this line

type ```i``` to insert

copy following code to paste

```plugins=(git zsh-autosuggestions zsh-completions zsh-syntax-highlighting)```

```autoload -U compinit && compinit```

Click ```ESC``` key and type ```:wq``` to save and quit.

- if network is'not very good, you better use nano to edit

```nano .zshrc```

find > delete > paste > save

---

## Good luck !
