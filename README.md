# HBC Workshop Demo
Drupal 10 project setup with Lando

## Requirements
You need to have these applications installed to operate on all environments:

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Lando](https://docs.lando.dev/install.html)

## Create and start the environment

```
# Startup the container
lando start

# Install composer packagers
lando composer install

# Import the dump.sql
lando db-import dump.sql

# Import configurations
lando drush cim

```
Ready! Now go to https://hbc-workshop-2024.lndo.site/ to see your site.


## Useful commands

List information about this app
```
lando info
```

Export database
```
lando db-export dump.sql
```

Export configs
```
lando drush cex
```
