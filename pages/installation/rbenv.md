---
layout: page
title: Rbenv
---

## Installation

```bash
$ brew install rbenv ruby-build
```



https://gist.github.com/brentertz/1384279  
https://gist.github.com/jpantuso/1110217  
http://www.bounga.org/ruby/2012/02/06/pow-using-rbenv/
http://robots.thoughtbot.com/using-rbenv-to-manage-rubies-and-gems

## Configuration

```bash
$ echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.zprofile
$ source ~/.zprofile
```

## Install ruby

```bash
$ rbenv install 2.1.1
$ rbenv global 2.1.1
```

```bash
$ gem update --system
```

## Config gem and install commons gem for rails dev

```bash
$ echo 'gem: --no-rdoc --no-ri' >> ~/.gemrc
```

```bash
$ gem install bundler foreman pg rails --no-rdoc --no-ri
```

## Rbenv plugins

```bash
brew install rbenv-gem-rehash rbenv-bundler
```

## Ruby and web tools

```bash
$ curl get.pow.cx | sh
```

## Databases

```bash
$ brew install [mysql] postgresql redis
```
