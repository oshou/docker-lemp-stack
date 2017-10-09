# docker-centos7-phpfpm

## 設定内容
- ロケール設定
- タイムゾーン設定
- ミドルウェアインストール
  - 運用ツール
  - NGINX
  - php-fpm
  - PHP関連ツール一式
  - アプリの設定登録
- yumキャッシュクリア
- 各ミドルウェアの設定ファイル配置
- 公開用ポートの設定
- スタートアップスクリプト実行(NGINX, php-fpm起動)

## 起動方法

```
$ docker run --name phpfpm -dit -p 80:80 -p 9000:9000 --privileged oshou/docker-centos7-phpfpm-php54:latest
$ docker exec -it phpfpm /bin/bash
```
