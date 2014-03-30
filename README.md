# Advanced PHP Heroku Build Pack
================================

This is a fork from https://github.com/CHH/heroku-buildpack-php to support Laravel 4.
For the full Readme, please refer to https://github.com/CHH/heroku-buildpack-php

## How to use it

Use the `--buildpack` parameter when creating a new app:

    heroku create --buildpack https://github.com/minhdanh/heroku-buildpack-php-1 myapp

Or set the `BUILDPACK_URL` config var on an existing app:

    heroku config:set BUILDPACK_URL=https://github.com/minhdanh/heroku-buildpack-php-1
    
* * *
Note: If you're deploying Laravel 4, you may want to write a database.php file to read information from DATABASE_URL, so you need to enable user-env-compile
    
    heroku labs:enable user-env-compile

* * *
