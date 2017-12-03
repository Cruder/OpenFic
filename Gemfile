# frozen_string_literal: true

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?('/')
  "https://github.com/#{repo_name}.git"
end

# Server
gem 'puma', '~> 3.7'
gem 'rails', '~> 5.1.4'

# Database
gem 'sqlite3'
# gem 'redis', '~> 3.0'

# Deploy
# gem 'capistrano-rails', group: :development

# API
# gem 'jbuilder', '~> 2.5'
# gem 'rack-cors'

# Code quality
gem 'overcommit', '~> 0.41.0'
gem 'rubocop', '~> 0.51.0', require: false

group :development, :test do
  # Debug
  gem 'byebug', platforms: %i[mri mingw x64_mingw]
end

group :development do
  # Cache
  gem 'listen', '>= 3.0.5', '< 3.2'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: %i[mingw mswin x64_mingw jruby]
