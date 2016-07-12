require "json"
require "open-uri"
source "https://rubygems.org"

deps = JSON.parse(open("https://pages.github.com/versions.json").read)
gem "github-pages", deps["github-pages"]
