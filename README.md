Default Project - Read Me
================

This is a default Ruby on Rails 4.0 project, using Ruby 2.0.0-p247. It is tested on OS-X 
Mountain Lion, with rbenv and uses bundler for gem management (via ~/.bundle/config).


Pre-requisites
------------

* OS-X Mountain Lion
* rbenv and binstubs plugin
* Ruby 2.0.0-p247
* Rails 4.0.0
* Postgresql
* Growl

Default Gems
-----------

### Database

* pg

### Layout/View

* haml-rails
* zurb-foundation

### Developoment/Testing Tools 

* guard-rspec
* guard-spork
* guard-livereload
* spork-rails
* rb-fsevent
* growl
* pry-rails
* better-errors
* binding_of_caller
* meta_request

### Testing

* rspec-rails
* factory_girl_rails
* faker
* capybara
* database_cleaner
* launchy
* selenium-webdriver
* shoulda-matchers

### Heroku (production)

* rails_12factor


Default configuration
-------------------

* Bundler run with binstubs to be installed at .bundle/bin

* run `rails generate rspec:install` 

* `--format-documentation` added to .rspec

* config/application.rb updated with rspec and factory_girl generator settings

* create Guardfile with settings for rspec, spork, growl and livereload

* update spec/spec_helper.rb with spork, factory_girl, capybara and database_cleaner settings

* replace application.html.erb with application.html.haml

* remove/test directory (as this causes conflicts with rspec, spork and guard)


Setup
------------

* Clone the repository `git clone [repo url] [new project name]`

* Remove git, run: `rm -rf .git`

* Update reference to `BaseProject` to new project name (via find and replace) 

* Create config/database.yml (see gist for format)

* Run `bundle install`

* Run `rbenv rehash` (to update the binstubs)

* Run `db:create:all`





<!-- Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions -->