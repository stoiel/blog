# drupal-docker-nginx
This is the Docker Compose environment to develop Drupal.

## Requirements
- Docker
- Docker Compose

## How to use
Copy and edit `.env`, `.env.docker`,
```zsh
% cp .env.example .env && cp .env.docker.example .env.docker
```

Export env vars,
```zsh
% export $(cat .env.docker | grep -v "^#" | xargs)
```

Then start the container.
```zsh
% docker-compose up -d
```

Install Composer packages.
```zsh
% docker-compose exec php composer install
```
