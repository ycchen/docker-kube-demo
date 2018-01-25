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

# Add Rspec and other gems to Gemfile
    gem 'rspec-rails'
    gem 'jquery-rails'
    gem 'bootstrap-sass'
    gem 'simple_form'
    gem 'faker'
    gem 'font-awesome-sass'
# Rspec generator
    rails g rspec:install
➜  rails-kube-demo git:(master) rails g rspec:install
Running via Spring preloader in process 10273
      create  .rspec
      create  spec
      create  spec/spec_helper.rb
      create  spec/rails_helper.rb
➜  rails-kube-demo git:(master) ✗ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

    .rspec
    spec/

# Simple Form generator
    rails g simple_form:install --bootstrap

➜  rails-kube-demo git:(master) ✗ rails g simple_form:install --bootstrap
Running via Spring preloader in process 10500
      create  config/initializers/simple_form.rb
      create  config/initializers/simple_form_bootstrap.rb
       exist  config/locales
      create  config/locales/simple_form.en.yml
      create  lib/templates/erb/scaffold/_form.html.erb
===============================================================================

  Be sure to have a copy of the Bootstrap stylesheet available on your
  application, you can get it on http://getbootstrap.com/.

  Inside your views, use the 'simple_form_for' with one of the Bootstrap form
  classes, '.form-horizontal' or '.form-inline', as the following:

    = simple_form_for(@user, html: { class: 'form-horizontal' }) do |form|
```