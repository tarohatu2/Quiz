source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end


# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.1.7'
# Use sqlite3 as the database for Active Record
# Use Puma as the app server
gem 'puma', '~> 3.7'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
# gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
gem 'redis', '~> 4.0'
# Use ActiveModel has_secure_password
gem 'bcrypt', '~> 3.1.7'

gem 'devise', "~> 4.5.0"
gem 'active_model_serializers'

# Use haml
gem 'haml-rails'

gem "pg", "~> 0.18"

# React Rails
gem 'react-rails'
gem 'webpacker', github: "rails/webpacker"

gem 'jbuilder', '~> 2.5'
# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

# Use Rack CORS for handling Cross-Origin Resource Sharing (CORS), making cross-origin AJAX possible
# gem 'rack-cors'

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'rspec-rails'
  gem "rspec_junit_formatter"
end

group :test do
  gem 'selenium-webdriver'  # CapybaraがSeleniumに依存しているため追加
  gem 'capybara', '~> 2.13'          # 英語に文法でRSpecにテストを記述できる
  gem 'factory_girl_rails'  # FactoryGirl追加
  gem 'cucumber-rails', :require => false # Cucumber追加
  gem 'database_cleaner', github: 'bmabey/database_cleaner' # Cucumber用にDBクリーナーを追加
end

group :development do
  gem "annotate"
  gem "better_errors"
  gem "binding_of_caller"
  gem "brakeman"
  gem "bullet"
  gem "listen", ">= 3.0.5", "< 3.2"
  gem "onkcop", require: false
  gem "rubocop"
  gem "web-console", ">= 3.3.0"
  gem "rails_best_practices", require: false
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
