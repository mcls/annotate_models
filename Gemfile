source 'https://rubygems.org'

ruby '>= 2.4.0'

gem 'activerecord', '>= 5.0.0', '< 8', require: false
gem 'rake', require: false

group :development do
  gem 'bump'
  gem 'mg', require: false
  gem 'travis', require: false
  platforms :mri, :mingw do
    gem 'yard', require: false
  end
end

group :development, :test do
  gem 'byebug'
  gem 'guard-rspec', require: false
  gem 'rspec', require: false

  gem 'rubocop', '~> 0.68.1', require: false unless RUBY_VERSION =~ /^1.8/
  # gem 'rubocop', '~> 1.12', require: false
  # gem 'rubocop-rake', require: false
  # gem 'rubocop-rspec', require: false
  # gem 'simplecov', require: false
  gem 'terminal-notifier-guard', require: false

  gem 'codeclimate-test-reporter'
  gem 'coveralls'

  gem 'overcommit'

  platforms :mri, :mingw do
    gem 'pry', require: false
    gem 'pry-byebug', require: false
  end
end

group :test do
  gem 'files', require: false
  gem 'git', require: false
end
