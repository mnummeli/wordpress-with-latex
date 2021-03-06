# Wordpress with LaTeX enabled for containers

## About

`texlive`-package added to Wordpress image in order to compile mathematical
formulas.

## Pre-requisities

* Recent enough Docker with Docker Compose enabled

## Build custom Wordpress

```
$ cd mywordpress
$ ./build.sh
```

## Start Wordpress

```
$ docker-compose up [-d]
```

## Web-addresses

For visiting your Wordpress site:

http://localhost:9080

For examining the MySQL database with Adminer

http://localhost:8080

See `docker-compose.yml` for default passwords.

## Enable LaTeX in Wordpress

Download some LaTeX-plugin like

https://fi.wordpress.org/plugins/wp-quicklatex/

In case of mentioned plugin, enable LaTeX sitewide from plugin's settings and
use `\[ ... \]` to enclose mathematical formulas.

## Stop Wordpress

```
$ docker-compose down
```

If you want to also remove the test content from database, issue

```
$ docker-compose down --volumes
```
