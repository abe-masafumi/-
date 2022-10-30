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