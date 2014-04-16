---
layout: page
title: Oh My Zsh
---

```bash
$ curl -L http://install.ohmyz.sh | sh
```

Update config

```bash
ZSH_THEME="nicolas-brousse"

...

plugins=(nicolas-brousse git osx rbenv brew brew-cask bundler colorize sublime rails pow lol gitignore github gem encode64 docker colored-man capistrano)

# Uncomment this line 
export ARCHFLAGS="-arch x86_64"
```

Create the theme

```bash
# ~/.oh-my-zsh/themes/nicolas-brousse.zsh-theme
local ret_status="%(?:%{$fg[cyan]%}➜ :%{$fg[red]%}➜ %s)"
PROMPT='${ret_status}%{$reset_color%}%c$(git_prompt_info) %{$fg[cyan]%}%#%{$reset_color%} '

ZSH_THEME_GIT_PROMPT_PREFIX=" (%{$fg[cyan]%}"
ZSH_THEME_GIT_PROMPT_SUFFIX="%{$reset_color%})"
ZSH_THEME_GIT_PROMPT_DIRTY="%{$fg[red]%}✗%{$reset_color%}"
```

Create plugin

```bash
# ~/.oh-my-zsh/plugins/nicolas-brousse/nicolas-brousse.plugin.zsh
p() { cd ~/Projects/$1; }
_p() { _files -W ~/Projects -/; }
compdef _p p
```

_Upgrade with: `upgrade_oh_my_zsh`_
