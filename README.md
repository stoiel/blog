# drupal-docker-nginx
This is the Docker Compose environment for developing Drupal app.

## Requirements
- Docker
- Docker Compose

## How to use
Copy and edit `.env` and `.env.docker`
```zsh
$ cp .env.example .env && cp .env.docker.example .env.docker
```

Export env vars.  
You can use make command.

```zsh
$ eval `make _init`
```

Then start the container.
```zsh
$ make upc
```

To install Composer packages, exec the following.
```zsh
$ docker-compose exec php composer install
```
