# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

* Create rails application without Test::Unit
```ruby
    rails new rails-kube-demo -T

# Add Rspec to Gemfile
    gem 'rspec-rails'

# Rspec generator
    rails g rspec:install
```