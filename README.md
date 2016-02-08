# phergie-freenode

## Warning

This is a fork of https://github.com/phergie/phergie-freenode for my personal
use. You are advised to reference the original repository since it is maintained
by the Phergie Team.

## Installation

* Copy `.env.example` to `.env`
* Run `composer install`
* Copy `config.php.example` to `config.php`
* Edit `config.php` to your preferences (Pay attention to each `# CHANGE ME`)
* To start Phergie run: `./vendor/bin/phergie config.php`

Optional (Deployment):

* Edit `Envoy.blade.php` to your server environment

Optional (Service):

* Edit `phergie.conf` to your server environment
* Copy `phergie.conf` to `/etc/init/phergie.conf`
* Run `service phergie restart`

## Deployment

* SSH into server
* Pull master from origin
* Composer install
* Restart phergie service

From the project root:

`./vendor/bin/envoy run deploy:prod`
