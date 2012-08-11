source "http://rubygems.org"

gem "rake"
gem "rails", "~> 3.0.0"
gem "paper_trail", "~> 2.0"
gem "will_paginate", "~> 3.0.pre2"

group *[:development, :test] do
  gem "capybara", ">= 0.4.0"
  gem "factory_girl_rails", "~> 1.1.beta1"
  gem "jeweler", "~> 1.8.4"
  gem "rdoc"
  gem "rspec-rails", "~> 2.5.0"
  gem "spork", "~> 0.9.0.rc"
  gem "sqlite3-ruby", :require => "sqlite3"

  # OPTIONAL LIBRARIES: These libraries upset travis-ci and may cause Ruby or
  # RVM to hang, so only use them when needed.
  if ENV['DEBUGGER']
    platform :mri_18 do
      gem 'rcov', :require => false
      gem 'ruby-debug'
    end

    platform :mri_19 do
      gem 'simplecov', :require => false
      gem 'debugger-ruby_core_source'
      gem 'debugger'
    end
  end
end
