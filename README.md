Introduction
------------
Example for deployment [CakePHP](http://cakephp.org) v2 [project](http://github.com/rikkeisoft/cakephp2) use [Deployer](http://deployer.org).

See [http://deployer.org](http://deployer.org) for more information and documentation about Deployer.
See [other example project](http://github.com/oanhnn/deployer-example)

Requirements
------------
* PHP 5.4.0 and up.

That's all!

You can install [ssh2 extension](http://php.net/manual/en/book.ssh2.php) to speedup deployment process and enable [sockets](http://php.net/manual/en/book.sockets.php) for parallel deployment.

Setting up [SSH agent forwarding](https://developer.github.com/guides/using-ssh-agent-forwarding/) if need.

Installation
------------
Clone with `git`
```shell
$ git clone git@github.com:rikkeisoft/deployer-cakephp2.git <target-directory>
$ cd <target-directory>
$ composer install
```
or using [`composer`](http://getcomposer.org)
```shell
$ composer create-project rikkeisoft/deployer-cakephp2 <target-directory>
```

Usage
-------------
Custom `stage/dev.php` or make copy with other stage for your system.    
First deployment:
```shell
$ bin/dep configure <stage>
$ bin/dep deploy <stage>
```

Second deployment and after:
```shell
$ bin/dep deploy <stage>
```

Contributing
------------
All code contributions must go through a pull request and approved by a core developer before being merged.
This is to ensure proper review of all the code.

Fork the project, create a feature branch, and send a pull request.

To ensure a consistent code base, you should make sure the code follows
the [PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md).

If you would like to help take a look at the [list of issues](https://github.com/rikkeisoft/deployer-cakephp2/issues).

License
-------
Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
