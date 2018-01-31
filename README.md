# docker_files
# dockerコンテナをバックグラウンド起動
docker-compose up -d
# コンテナの起動
docker-compose ps
docker ps -a
# コンテナに接続
docker exec -it CONTAINER ID bash
# node.js パッケージインストール アプリ起動
cd /app
npm install
npm start