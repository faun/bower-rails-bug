#Bower-rails bug

To reproduce, run `RAILS_ENV=production rake assets:precompile --trace`.

To work around this issue, run `rm vendor/assets/bower_components/**/*.js.{gzip,map}` and then run `RAILS_ENV=production rake assets:precompile`
