source "https://rubygems.org"

gemspec

if RUBY_VERSION == "1.8.7"
  gem "rake", "~> 10.5"
else
  gem "rake", ">= 11"
end

# Use local copy of simplecov in development when checked out, fetch from git otherwise
if File.directory?(File.dirname(__FILE__) + "/../simplecov")
  gem "simplecov", :path => File.dirname(__FILE__) + "/../simplecov"
else
  gem "simplecov", :git => "https://github.com/colszowka/simplecov"
end

group :test do
  gem "minitest"
end

group :development do
  gem "rubocop"
  gem "sass"
  gem "sprockets"
end
