source 'https://rubygems.org'

ruby '4.0.5'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'rails', '8.1.3'
gem 'pg', '~> 1.6'
gem 'puma', '>= 5.0'
gem 'sprockets-rails'
gem 'terser'
gem 'turbolinks', '~> 5'
gem 'jbuilder', '~> 2.5'
gem 'rails-i18n'


group :development, :test do
  gem 'byebug', platforms: %i[mri windows]
  gem 'capybara', '~> 3.40'
  gem 'selenium-webdriver'
  gem 'pry-rails'
  gem 'faker'
  gem 'rspec-rails', '~> 6.1.5'
  gem 'database_cleaner'
  gem 'factory_bot_rails'
  gem 'rexml'
end

group :development do
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '~> 3.9'
end

group :test do
  gem 'rails-controller-testing'
  gem "shoulda-matchers"
end

gem 'tzinfo-data', platforms: %i[windows jruby]
