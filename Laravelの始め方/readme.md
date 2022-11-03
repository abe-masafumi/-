# Laravelno始め方

[ドキュメント](https://laravel.com/docs/9.x/migrations#generating-migrations)

[ドキュメント](https://readouble.com/laravel/9.x/ja/installation.html)

## 開発環境 ローカル
- Mac(PC)上に構築する　＝>MAMP

## 開発環境 仮想環境
- Vargant + VirtualBox

- Docker


## ローカル環境で構築
- Mac(PC)上に構築する　＝>MAMP

- Composerが必要

- 色々インストールする前に"brew upgrade"[Homebrewで覚えておくと便利なコマンド一覧](https://parashuto.com/rriver/tools/homebrew-most-used-commands)を実行

- [プロジェクトの作成](https://laravel.com/docs/9.x)

## プロジェクトのディレクトリ構成

<img src="./image/img004.png">

## プロジェクトの環境設定

- .envでDBと接続設定

<img src="./image/img001.png">

- 文字コード設定

<img src="./image/img002.png">

- 詳細設定

<img src="./image/img003.png">

- マイグレーションのとは

<img src="./image/img005.png">

- マイグレーションの生成

<img src="./image/img006.png">

"migrations/"の中にフォルダを作成
```bush
php artisan make:migration create_owners_table
```

接続しているDBにテーブルを生成
```bush
php artisan migrate
```


## Docker環境で構築

Docker Desktopのインストール
[Download Docker Desktop](https://docs.docker.com/desktop/mac/apple-silicon/)

"Homebrew"でインストールしようとしたが、Docker　Desktopだげがインストールできるか不安だったのでwebからダウンロードした

Dockerがインストールできているか確認
```
docker -v

docker compose -v
```

vscodeの拡張機能で"Dcker"をインストール

## Docker Desktopの使い方

[document](https://docs.docker.jp/)


一度チュートリアルをやってみるといい

## 手順

ローカルでプロジェクトを作成

コマンド

```bush

```



## sailでlaravelの環境構築

https://qiita.com/goemontech/items/63c8de2a122a4bdb7967

```bush
プロジェクト立ち上げ
curl -s "https://laravel.build/example-app?with=mysql" | bash

プロジェクトに移動
cd example-app

Sail を既存のアプリケーションにインストールする
composer require laravel/sail --dev

＊ composer.jsonが更新される
＊ composer.lockが更新される

<!-- Sailのdocker-compose.ymlファイルをアプリケーションのルートに発行
php artisan sail:install

* docker-compose.yml
* phpunit.xml -->

プロジェクトの起動
./vendor/bin/sail up -d

Sailのdocker-compose.ymlファイルをアプリケーションのルートに発行
php artisan sail:install --devcontainer

* "docker-compose.yml"の作成
* "phpunit.xml"の作成
* ".devcontainer/devcontainer.json"の作成

プロジェクトの停止
./vendor/bin/sail stop

sailのバージョン確認
sail php --version
```