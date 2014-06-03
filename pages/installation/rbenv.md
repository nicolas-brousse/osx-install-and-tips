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


## Install ruby

```bash
$ rbenv install 2.1.2
# Define ruby 2.1.2 as default
$ rbenv global 2.1.2
```

```bash
$ gem update --system
```

## Config gem and install commons gem for rails dev

```bash
$ echo 'gem: --no-rdoc --no-ri' >> ~/.gemrc
```

```bash
$ gem install bundler foreman pg rails
```

## Rbenv plugins

```bash
brew install rbenv-gem-rehash rbenv-bundler
```

## Pow.cx - zero-config Rack server

```bash
$ curl get.pow.cx | sh
```
