source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?('/')
  "https://github.com/#{repo_name}.git"
end

gemspec

gem 'rails', github: 'rails'
gem 'sqlite3', platforms: [:ruby]
gem 'activerecord-jdbcsqlite3-adapter', platforms: [:jruby]
gem 'activerecord-import'
gem 'uniform_notifier', git: "https://github.com/klaxit/uniform_notifier.git",
                        ref: "5f3a345ea9e634b9369dac6edcc3fb9a4ac8a184"

gem 'rspec'
gem 'guard'
gem 'guard-rspec'

gem 'coveralls', require: false

platforms :rbx do
  gem 'rubysl', '~> 2.0'
  gem 'rubinius-developer_tools'
end
