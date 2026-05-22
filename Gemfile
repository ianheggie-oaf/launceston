# frozen_string_literal: true

# It's easy to add more libraries or choose different versions. Any libraries
# specified here will be installed and made available to your morph.io scraper.
# Find out more: https://morph.io/documentation/ruby

source "https://rubygems.org"

ruby "3.2.2"

gem "mechanize", "~> 2.8.5"
# heroku-18 (glibc 2.23) platform can't run nokogiri >= 1.17 precompiled gems (require glibc 2.28).
# Pinned until morph.io upgrades its stack. bundle-audit will complain - known/accepted.
# .github/dependabot.yml tells it to ignore versions >= 1.17.0
gem "nokogiri", "~> 1.16.8" # Latest version the platform supports
gem "rake", "~> 12.3"
gem "rspec", "~> 3.0"
gem "rubocop"
gem "scraperwiki", git: "https://github.com/openaustralia/scraperwiki-ruby.git", branch: "morph_defaults"
gem "simplecov", "~> 0.18.0"
gem "simplecov-console"
gem "sqlite3", "~> 1.6.3"
