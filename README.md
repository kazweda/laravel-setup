# laravel-setup
```sh
/bin/bash -c "$(curl -fsSL https://php.new/install/mac/8.4)"
```
PHP、Composer、Laravelがインストールされる。
```sh
source ~/.zshrc
```

### プロジェクトを作成
```sh
laravel new example-app
```
#### starter kit
- none
#### database
- SQLite

### 起動
```sh
cd example-app
composer run dev
```
ブラウザで開いてみる。
http://127.0.0.1:8000

### Devcontainerの使用
https://readouble.com/laravel/12.x/ja/sail.html#configuring-a-shell-alias

もし、Devcontainer内で開発したい場合は、--devcontainerオプションをsail:installコマンドで指定してください。
--devcontainerオプションは、sail:installコマンドに、デフォルトの.devcontainer/devcontainer.jsonファイルを
アプリケーションのルートにリソース公開するように指示します。

```sh
php artisan sail:install --devcontainer
```
### sailの準備
```sh
composer require laravel/sail --dev
```
### サービスの追加
```
php artisan sail:install
```
- mysql
- redis
- selenium
- meilisearch
- mailpit
を選択

コンテナの構築が始まる。（しばらくかかります）
### サービスの起動
```sh
sail up -d
```

