Grape API on Haoke
=================


A [Grape](http://github.com/intridea/grape) API mounted on Haoke.

$ bundle install --path vendor/bundle
$ bundle install --binstubs
$ bin/rackup
$ or bin/shotgun -d
$ or bin/tux

Description
$ bundle
$ bin/rake -T
$ bin/rake db:migrate


Loading NewRelic in developer mode ...
[2013-06-20 08:57:58] INFO  WEBrick 1.3.1
[2013-06-20 08:57:58] INFO  ruby 1.9.3 (2013-02-06) [x86_64-darwin11.4.2]
[2013-06-20 08:57:58] INFO  WEBrick::HTTPServer#start: pid=247 port=9292
```

### Hello World

Navigate to http://localhost:9292/api/v1/hello with a browser or use `curl`.

```
$ curl http://localhost:9292/api/v1/hello


New Relic
---------

The application is setup with NewRelic w/ Developer Mode. Navigate to http://localhost:9292/newrelic after making some API calls.
