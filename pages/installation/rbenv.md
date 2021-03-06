---
layout: page
title: Rbenv
---

## Installation

```bash
$ brew install rbenv ruby-build
```

## OhMyZsh

Add the `rbenv` plugin to OhMyZsh config.

## Install ruby

```bash
$ rbenv install 2.4.1
# Define ruby 2.4.1 as default
$ rbenv global 2.4.1
```

```bash
$ gem update --system
```

## Config gem and install commons gem for rails dev

```bash
$ echo 'gem: --no-document' >> ~/.gemrc
```

```bash
$ gem install bundler foreman pg rails
```

```bash
# Parallelize gems installation with bundle
$ bundle config --global jobs `expr $(sysctl -n hw.ncpu) - 1`
```

## Puma-dev - local proxy for rack applications

```bash
$ brew install puma/puma/puma-dev
```

## Tips

Somes tips [here]({{ site.baseurl }}/pages/tips/rbenv).

---

#### Links

https://gist.github.com/brentertz/1384279  
https://gist.github.com/jpantuso/1110217  
http://www.bounga.org/ruby/2012/02/06/pow-using-rbenv/
http://robots.thoughtbot.com/using-rbenv-to-manage-rubies-and-gems
https://robots.thoughtbot.com/parallel-gem-installing-using-bundler
