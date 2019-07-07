# drupal-docker-nginx
Docker Composeを用いたDrupalの開発環境です。  

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

### Composerモジュールのインストール
```bash
$ docker-compose exec php composer install
```  
