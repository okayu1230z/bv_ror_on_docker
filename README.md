# BootstrapVue + RoR on Docker

BootstrapVue (^4.6.0) & Vue.js (^2.6.11) & Ruby on Rails (^6.0.0) & MySQL (8.0) development environment on Docker

# How to setup

Please exec:

`$ docker-compose run frontend npm install @vue/cli bootstrap-vue bootstrap`

Please edit Dockerfile, Uncomment out:

```
COPY package.json .
```

Finally,

`$ docker-compose up`

After that, please docker-compose up every time you execute it.

# Maintenance

If you want to run bundle install:

`$ docker-compose run web bundle install`

If you want login frontend container:

`$ docker-compose run front sh`

If you want to webpacker's install command:

`$  docker-compose run backend rails webpacker:install`

If you see this error `ActiveRecord::NoDatabaseError`:

`$ docker-compose run backend rails db:create`
