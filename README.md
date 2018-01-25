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

# Generate scaffold for User model
 rails g scaffold User first_name last_name email

 Running via Spring preloader in process 10582
      invoke  active_record
      create    db/migrate/20180125161805_create_users.rb
      create    app/models/user.rb
      invoke    rspec
      create      spec/models/user_spec.rb
      invoke  resource_route
       route    resources :users
      invoke  scaffold_controller
      create    app/controllers/users_controller.rb
      invoke    erb
      create      app/views/users
      create      app/views/users/index.html.erb
      create      app/views/users/edit.html.erb
      create      app/views/users/show.html.erb
      create      app/views/users/new.html.erb
      create      app/views/users/_form.html.erb
      invoke    rspec
      create      spec/controllers/users_controller_spec.rb
      create      spec/views/users/edit.html.erb_spec.rb
      create      spec/views/users/index.html.erb_spec.rb
      create      spec/views/users/new.html.erb_spec.rb
      create      spec/views/users/show.html.erb_spec.rb
      create      spec/routing/users_routing_spec.rb
      invoke      rspec
      create        spec/requests/users_spec.rb
      invoke    helper
      create      app/helpers/users_helper.rb
      invoke      rspec
      create        spec/helpers/users_helper_spec.rb
      invoke    jbuilder
      create      app/views/users/index.json.jbuilder
      create      app/views/users/show.json.jbuilder
      create      app/views/users/_user.json.jbuilder
      invoke  assets
      invoke    coffee
      create      app/assets/javascripts/users.coffee
      invoke    scss
      create      app/assets/stylesheets/users.scss
      invoke  scss
      create    app/assets/stylesheets/scaffolds.scss
```