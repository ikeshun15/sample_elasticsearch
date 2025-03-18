# 🔍 Sample Elasticsearch


## 初期設定
### 1. 環境変数設定用の`.env`ファイル作成

1. `.env_sample`ファイルをコピーして、`.env`に名前を変更する

2. 必要な環境変数を入力して、保存する


### 2. 日本語プラグインをインストールしたカスタムイメージを作成する

```bash
docker build -t ikeshun15/elasticsearch:8.17.1 .
```


## 起動・終了手順
### Elasticsearch, Kibana

#### コンテナ立ち上げ

```bash
cd main_modules
docker compose up -d
```

#### コンテナ立ち下げ

```bash
docker compose down
```

### Connector
```bash
cd connectors
docker compose up -d
```

#### コンテナ立ち下げ

```bash
docker compose down
```

Created by 🍓