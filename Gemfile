source "https://rubygems.org"

gemspec

group :development do
  gem "rake"
  gem "rake-compiler"
  gem "test-unit", "~> 3.0", ">= 3.4.6"
  gem "test-unit-ruby-core"
  # In the case of Ruby whose rdoc is not a default gem.
  # Avoid installing rdoc gem in GitHub Actions as a workaround.
  # https://github.com/ruby/openssl/issues/699
  gem "rdoc" unless ENV["CI"] == "true"
end
