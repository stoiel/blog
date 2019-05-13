# myblog
Docker Composeを用いて構築したブログです。アプリケーションはDrupalを使用しています。

## 構築手順
`.env`を編集します。

```bash
$ cp .env.example .env
$ cp .env.docker.example .env.docker
```

ターミナルで下記を実行します。

```bash
$ docker-compose up -d
```

---
## English:

this is my blog using Drupal and Docker Compose.

## Prerequisites
This project is intended to be used on Docker container.

## Usage
Exec the following command

```bash
$ docker-compose up -d
```
