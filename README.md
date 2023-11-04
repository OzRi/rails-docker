# 環境構築手順

## 1. リポジトリをクローン
```
git clone <Repository URL>
cd rails-docker
```

## 2. アプリを起動する
```
docker-compose up -d
```

## 3. DBのセットアップ
```
docker-compose exec web bash
rails db:create
rails db:migrate
```

## 4. アプリに接続する
ブラウザで以下の接続先へアクセスする
```
http://localhost:3000/
```