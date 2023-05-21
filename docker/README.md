# Laravel環境構築

## 環境変数について

環境変数の利用には`.env`ファイルが必要です。

リポジトリの`.env.example`をコピーして該当ファイルを作成してください。

## Build & Up

`docker-compose up -d --build`

## コンテナ起動状態を確認

`docker-compose ps`

コンテナが2つ立ち上がっていればOK

## Package Install

appコンテナに入る  
`docker-compose exec app bash`

### WSL2 in Windows

`docker compose exec -u1000:1000 app bash`

## Laravelプロジェクト作成

`composer create-project --prefer-dist laravel/laravel . "9.x"`

