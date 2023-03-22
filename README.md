# Grafana + Prometheus + nginx + docker による監視システムの構築

## 前提条件

- docker / docker-compose
- ホスト環境の /etc/letsencrypt に let's encrypt証明書が取得済みであること

## 使用方法

- `.env`の内容を環境に合わせて調整する

```.env

# GrafanaへアクセスするためのHTTPDポート指定
PORT=18443

# サーバ名の指定
NGINX_SERVER_NAME=art-ai-backend.maxcorporation.app

```

- コンテナを起動する

```sh
docker-compose up -d
```
