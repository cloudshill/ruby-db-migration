
$ bundle install --path vendor/bundle
$ bundle install --binstubs
$ bundle
$ bin/rake -T
# connect database test
bin/rake db:connect_db
# create database, ENV_RACK=production(default development) bin/rake db:create
bin/rake db:create
# create migration 
rake db:create_migration NAME=migration_name
ex. : rake db:create_migration NAME=create_users

$ bin/rake db:migrate
