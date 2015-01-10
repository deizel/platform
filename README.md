# Platform for CakePHP 3 Web Application

A skeleton to quickly cook some _gourmet_ [CakePHP][cakephp] web apps.

> __NOTE:__ Platform is in alpha, [missing some important packages](#TODO) but ready to help
> you quickly get started with your [CakePHP 3][cakephp] application.

## But Why?

Put simply, the official app skeleton is very basic (and rightfully so).

Platform, while replicating the official app skeleton as much as possible, distinguishes itself by a few structural
changes, some pre-installed/configured libraries/plugins and some 'best practices'.

## Pre-installed packages

### Composer

* [cakephp/cakephp][cakephp/repo] to power the application.
* [cakephp/debug_kit][debug_kit/repo] - the official CakePHP debugging tool.
* [cakephp/migrations][migrations/repo] - the official CakePHP migrations shell.
* [friendsofcake/bootstrap-ui][foc/bootstrap-ui/repo] to quickly get things going.
* [friendsofcake/crud][foc/crud/repo] to quickly get things going.
* [gourmet/faker][faker/repo] to generate fixture and seed data.
* [gourmet/robo][robo/repo] to run build or other tasks using [Robo][robo].
* [josegonzalez/dotenv][dotenv/repo] to easily manage environment variables.
* [markstory/asset_compress][asset_compress/repo] to handle asset compression, minification, etc.
* [mobiledetect/mobiledetectlib][mobiledetect/repo].

##### Developer mode

* [codeception/codeception][codeception/repo] to run acceptance, functional and unit tests ([sebastianbergmann/phpunit][phpunit/repo] included).
* [codeception/specify][specify/repo] BDD code blocks for PHPUnit and Codeception.
* [codeception/verify][verify/repo] BDD assertion library for PHPUnit.
* [d11wtq/boris][boris/repo]
* [gourmet/whoops][whoops/repo] to beautify errors and exceptions (only in debug mode)

### Bower

* [twbs/bootstrap][bootstrap]
* [jquery/jquery][jquery]

## Get started

It is assumed that you have the following installed globally:

* [Composer][composer] - PHP package manager
* [Bower][bower] - Front-end package manager

If (or once) you have them all installed, run:

```
composer create-project -s dev gourmet/platform [app_name]
```

_You might want to check out `[Gourmet/Box][gourmet/box]` if you prefer using a self contained setup._

## Configure

Platform's configuration is broken into 'scopes':

* application
* asset_compress
* cache
* database
* dispatcher
* email
* error
* log
* paths
* plugin
* routes
* security
* session

This makes configuration a little more organized (compared to a single bloated file) and easily accessible using your
IDE's fuzzy finder (try typing 'log' in the fuzzy finder, the first matching file should the log config file).

### Quick Tips

To enable `debug` mode without having to modify any file:

```
touch .debug
```

## TODO

* [ ] Use [gourmet/twitter_bootstrap][twitter_bootstrap/repo] to make CakePHP helpers play well with Twitter Bootstrap.
* [ ] Use [monolog/monolog][monolog/repo] to handle all types of logging. See [#2033][cakephp/2033].
* [x] Use [cakephp/debug_kit][debug_kit/repo] once it is released for CakePHP 3.
* [x] Use [cakephp/migrations][migrations/repo] once it is released for CakePHP 3.
* [x] Add link to virtual machine information.
* [ ] Add link to [capcake][capcake/repo] deployments.
* [ ] Add link to [rocketeer][rocketeer/repo] deployments.

## Versioning

Platform uses [semantic versioning][semver]:

> Given a version number MAJOR.MINOR.PATCH, increment the:
>
> - MAJOR version when you make incompatible API changes,
> - MINOR version when you add functionality in a backwards-compatible manner, and
> - PATCH version when you make backwards-compatible bug fixes.
>
> Additional labels for pre-release and build metadata are available as extensions to the
> MAJOR.MINOR.PATCH format.

## License

Copyright (c) 2015, Jad Bitar and licensed under [The MIT License][mit].

[asset_compress/repo]://github.com/markstory/asset_compress
[bootstrap]:http://getbootstrap.com
[boris/repo]://github.com/d11wtq/boris
[bower]:http://bower.io
[cakephp]:http://cakephp.org
[cakephp/2033]://github.com/cakephp/cakephp/issues/2033
[cakephp/repo]://github.com/cakephp/cakephp
[capcake/repo]://github.com/jadb/capcake
[codeception/repo]://github.com/codeception/codeception
[composer]://getcomposer.org/doc/00-intro.md#globally
[debugbar/repo]://github.com/maximebf/debugbar
[debug_kit/repo]://github.com/cakephp/debug_kit
[dotenv/repo]://github.com/josegonzalez/php-dotenv
[faker/repo]://github.com/gourmet/faker
[foc/bootstrap-ui/repo]://github.com/friendsofcake/bootstrap-ui
[foc/crud/repo]://github.com/friendsofcake/crud
[gourmet/box]://github.com/gourmet/box/
[jquery]:http://jquery.com
[milestones]://github.com/gourmet/platform/issues/milestones
[migrations/repo]://github.com/cakephp/migrations
[mit]:http://www.opensource.org/licenses/mit-license.php
[mobiledetect/repo]://github.com/mobiledetectlib/mobiledetectlib
[monolog/repo]://github.com/seldaek/monolog
[phinx/repo]://github.com/robmorgan/phinx
[phpunit/repo]://github.com/sebastianbergmann/phpunit
[puppet]:https://puppetlabs.com
[puphpet]:https://puphpet.com
[robo]:http://robo.li
[robo/repo]://github.com/gourmet/robo
[rocketeer/repo]://github.com/anahkiasen/rocketeer
[semver]:http://semver.org
[specify/repo]://github.com/codeception/specify
[twitter_bootstrap/repo]://github.com/gourmet/twitter_bootstrap
[vagrant]:http://vagrantup.com
[verify/repo]://github.com/codeception/verify
[whoops/repo]://github.com/gourmet/whoops
