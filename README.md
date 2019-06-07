# wp-plugin-ngp

Basic overview:
  Composer is used to install project dependencies and for
  package distribution via https://wpackagist.org/. Docker
  is used for local development via any running container
  daemon (Vagrant inlcuded for ease of use)


# Running

### Composer
Used to install dependencies and you have two options to use composer [locally, docker]

Locally installed
```
composer install
```

Docker
```
docker-compose -f docker-composer-installer.yml up

#or

docker run -v "$(pwd)":/app composer install
```

### DevOps
To get a local setup running you have two options, docker or vagrant

Docker-Compose
```
docker-compose up
```
Vagrant
```
vagrant up
```


# Misc/Disclaimers
  Some generic info here about the project

## Links
  - https://www.php.net/manual/en/install.php
  - https://getcomposer.org/download/
  - https://docs.docker.com/compose/install/
  - https://www.vagrantup.com/downloads.html
  - https://www.virtualbox.org/wiki/Downloads