---
layout: page
title: Homebrew
---

## Homebrew installation

```bash
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew update
```

## Install commons

```bash
$ brew install openssl
$ brew install wget
$ brew install curl tree git
$ brew install bash zsh
# $ brew install ossp-uuid ssh-copy-id
$ brew install vim
$ brew install imagemagick jpegoptim
$ brew install ffmpeg
$ brew install node
$ brew install heroku-toolbelt
```

## Databases

```bash
$ brew install postgresql [mysql] [sqlite]
$ brew install redis memcached
```

Now we lock the database formulae to avoid auto update.

```bash
$ brew pin postgresql [mysql] [sqlite]
```


## Checks all is good

```bash
$ brew doctor
```

## Tips

Somes tips [here]({{ site.baseurl }}/pages/tips/homebrew).

---
#### Links

- http://robots.thoughtbot.com/starting-and-stopping-background-services-with-homebrew
- http://robots.thoughtbot.com/brewfile-a-gemfile-but-for-homebrew

```bash
$ brew install android-sdk
$ brew install automysqlbackup ??

$ brew install zsh......
```
