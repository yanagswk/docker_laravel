## 実行環境
- php: php: 7.4-fpm-buster
- composer: 2.0
- nginx: 1.18-alpine
- mysql/mysql-server: 8.0
- Laravel: 6.x
- docker
- docker-compose

## Laravelインストール  
- アプリケーションサーバーのコンテナに入る
`docker-compose exec app bash`  

- Laravel version8インストール
`composer create-project --prefer-dist "laravel/laravel=6.*" .`
`create-project`は空っぽのディレクトリにしか実行できない。

## docker コマンド
コンテナ内に入る  
`docker-compose exec [サービス名] bash`  

コンテナに入らなくても、コマンドは実行できる  
`docker-compose exec [サービス名] [コマンド]`

## memo
Laravel公式にnginxの設定例が用意されている  
[Laravel公式 ver8](https://readouble.com/laravel/8.x/ja/deployment.html)  

## 参考文献
[【超入門】20分でLaravel開発環境を爆速構築するDockerハンズオン](https://qiita.com/ucan-lab/items/56c9dc3cf2e6762672f4#docker%E7%92%B0%E5%A2%83%E3%81%AE%E5%86%8D%E6%A7%8B%E7%AF%89)  

[docker-composeでLaravel6×MySQL×Nginx環境構築](https://niwakatech.info/laravel-docker-compose/)
