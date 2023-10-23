# Deanin Ruby On Rails r/place clone speedrun

Youtube: Realtime r/place Clone Speedrun in Ruby on Rails 7
https://www.youtube.com/watch?v=aZq_pU2dysk

## Build the app

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
```

## Launch the app

```bash
rails s
# then open two browsers and log at user1@example.com and user2@example.com to see the change live
```
