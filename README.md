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
