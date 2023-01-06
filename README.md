# lara9-sample

## 概要
Laravel9のサンプルプロジェクトです。

## 環境構築

`$cd [cloneしたプロジェクト]`\
- `.env.sample`ファイルをコピーして同階層に`.env`ファイルを作成してください。

makefileに実行コマンドを記載しています。以下コマンドを実行してください。
- 初期インストール\
`$ make install`
- 停止\
`$ make down`
- 再起動\
`# make up`

- laravelプロジェクトに移動してcomposer installします\
`$ make app`\
`data# composer install`
- npmを起動します\
`data# exit`\
`$ cd src`\
`$ npm install`\
`$ npm run dev`\
`/`画面の右上からログイン画面に遷移できればOKです

## DBクライアントツールで接続したい場合
- dbのportは3306で設定しています
- その他の設定は`.env`記載の通り接続ください
- portを変更したい場合は、`docker-compose.yml`のdbのport行でportを変更して、コンテナを再起動してください

## その他
環境構築は以下のサイトを参考にしています。\
https://qiita.com/ucan-lab/items/56c9dc3cf2e6762672f4#%E8%A3%9C%E8%B6%B3mysql%E3%82%AF%E3%83%A9%E3%82%A4%E3%82%A2%E3%83%B3%E3%83%88%E3%83%84%E3%83%BC%E3%83%AB%E3%81%A7%E6%8E%A5%E7%B6%9A%E3%81%97%E3%81%9F%E3%81%84

### breeze
認証はbreezeを利用しています。\
（日本語化は[Laravel-Lang](https://github.com/Laravel-Lang/lang)）\
参考：https://specially198.com/implement-user-registration-and-login-with-breeze-of-laravel9/

### mailhogについて
参考：https://logsuke.com/web/programming/laravel/laravel-mailhog \
http://localhost:8025/ で受信画面が開けることができればOK

### ably（ブロードキャスト・サービス）
https://ably.com/

無料枠は、2022.08.31 現在で「600万／月」メッセージ

参考:https://blog.capilano-fw.com/?p=10909# lara9-react-chat
