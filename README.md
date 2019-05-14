# myblog
Docker Composeを用いて構築したブログです。アプリケーションはDrupalを使用しています。

## 構築手順
`.env`を編集します。

```bash
$ cp .env.example .env
$ cp .env.docker.example .env.docker
```

事前に`.env.docker`を展開しておきます。
```bash
$ export $(cat .env.docker | grep -v "^#" | xargs)
```

ターミナルで下記を実行してコンテナを立ち上げます。
```bash
$ docker-compose up -d
```

---
## English:

this is my blog using Drupal and Docker Compose.

## Prerequisites
This project is intended to be used on Docker container.

## Usage
Copy and Edit the `.env`.

```bash
$ cp .env.example .env
$ cp .env.docker.example .env.docker
```

Export variables declared in the `.env.docker`.
```bash
$ export $(cat .env.docker | grep -v "^#" | xargs)
```

Exec the following command.
```bash
$ docker-compose up -d
```
