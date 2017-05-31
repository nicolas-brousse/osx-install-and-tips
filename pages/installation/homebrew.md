---
layout: page
title: Homebrew
---

## Homebrew installation

```bash
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew update
```

## Add some Homebrew repositories

```bash
$ brew tap homebrew/bundle
$ brew tap homebrew/services
```

## Install commons

```bash
$ brew install openssl
$ brew install wget curl tree htop
$ brew install git git-lfs git-extras gist
$ brew install bash zsh
# $ brew install ossp-uuid
$ brew install ssh-copy-id duck
$ brew install vim macvim
$ brew install imagemagick jpegoptim
$ brew install node yarn
$ brew install ffmpeg --with-x265

$ brew install scw # Scaleway.com CLI
$ brew install forego

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
