# Web App

This web app consist in a blog which allows the application of the CRUD model in articles. It has different categories and users, who have different levels of permissons.

## Software Versions
* Ruby 2.7.2
* Rails 5.1.7

### Clone repo

In order to clone this project, you need to put the following into git bash

> git clone https://github.com/ezequielmura/webapp_prueba.git

### Initial settings

You need to create a database.yml. I leave you the example I used
```# SQLite version 3.x
#   gem install sqlite3
#
#   Ensure the SQLite 3 gem is defined in your Gemfile
#   gem 'sqlite3'
#
default: &default
  adapter: sqlite3
  pool: 5
  timeout: 5000
  

development:
  <<: *default
  database: db/development.sqlite3

# Warning: The database defined as "test" will be erased and
# re-generated from your development database when you run "rake".
# Do not set this db to the same as development or production.
test:
  <<: *default
  database: db/test.sqlite3

production:
  adapter: postgresql
  encoding: unicode
  pool: <%= ENV.fetch("RAILS_MAX_THREADS") { 5 } %>
  url: <%= ENV['DATABASE_URL'] %>
```
After this you need to execute
>bundle install
>rails server

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
