# Deanin Ruby On Rails r/place clone speedrun (in Docker env)

Actioncable + Stimulus

```bash
rails new deanin-rails-rplace-clone-speedrun && cd deanin-rails-rplace-clone-speedrun && code .
bundle add devise
rails g devise:install
rails g devise User
rails g model pixel x:integer y:integer color:string user:references
rails g stimulus pixels
rails g channel pixels
rails g controller pages home
rails g controller pixels
rails db:migrate
# Edit db/seeds.rb
rails db:seed
rails s
```

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
