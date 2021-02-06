# BootstrapVue + RoR on Docker

BootstrapVue (^4.6.0) & Vue.js (^2.6.11) & Ruby on Rails (~> 6.0.3) & MySQL (8.0) development & production environment on Docker

# How to setup

Please exec:

`$ docker-compose up`

# Maintenance

If you want to run bundle install:

`$ docker-compose run web bundle install`

If you want login frontend container:

`$ docker-compose run front sh`

If you want to webpacker's install command:

`$  docker-compose run backend rails webpacker:install`

If you see this error `ActiveRecord::NoDatabaseError`:

`$ docker-compose run backend rails db:create`

If you see this error `bootstrap-vue in ./src/main.js`

`docker-compose run frontend npm install --save boostrap-vue bootstrap`