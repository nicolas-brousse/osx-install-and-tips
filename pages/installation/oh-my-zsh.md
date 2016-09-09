---
layout: page
title: Oh My Zsh
---

```bash
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Update config

```bash
ZSH_THEME="nicolas-brousse"

...

plugins=(nicolas-brousse git osx rbenv brew brew-cask bundler colorize atom rails lol gitignore github gem encode64 docker colored-man capistrano xcode vagrant systemadmin battery ssh-agent)

# Uncomment this line
export ARCHFLAGS="-arch x86_64"
```

### Create the theme

```bash
# ~/.oh-my-zsh/custom/themes/nicolas-brousse.zsh-theme
local ret_status="%(?:%{$fg[cyan]%}➜ :%{$fg[red]%}➜ %s)"
PROMPT='${ret_status}%{$reset_color%}%c$(git_prompt_info) %{$fg[cyan]%}%#%{$reset_color%} '

ZSH_THEME_GIT_PROMPT_PREFIX=" (%{$fg[cyan]%}"
ZSH_THEME_GIT_PROMPT_SUFFIX="%{$reset_color%})"
ZSH_THEME_GIT_PROMPT_DIRTY="%{$fg[red]%}✗%{$reset_color%}"

```

### Create plugin

```bash
# ~/.oh-my-zsh/custom/plugins/nicolas-brousse/nicolas-brousse.plugin.zsh
_p() { _files -W ~/Projects -/; }

# Alias
alias jekyllserve="jekyll serve -w -D --future -b ''"

alias gt="gittower"
alias gtt="gittower ."
alias gti="gittower --init"

alias at="atom"
alias att="atom ."

alias sha256sum="shasum -a 256"


p() { cd ~/Projects/$1; }
compdef _p p
pat() { at ~/Projects/$1; }
compdef _p pat

```

#### Commands

`upgrade_oh_my_zsh`: upgrade oh my zsh
