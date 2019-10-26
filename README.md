# wwa-next
[WWAWing](https://github.com/WWAWing/WWAWing) の [MessageQueue問題](https://github.com/WWAWing/WWAWing/issues/129) に対応すべく、 WWA Wing のイベント実行モデルの再設計・リファクタリングを行うまつゆきの個人プロジェクトです。

このプロジェクトは WWA Wing Team のものではなく、まつゆき個人のものです。

## 開発方針
  - 高速開発
  - 予告なく、機能が増えたり減ったりする。
  - Java版互換完全無視。
  - WWA Wing の developブランチを取り込み続ける。
  - WWA Wing へのマージは「一旦考えない」。
    - ただし、すぐ使える成果が得られれば入れることも考える。
  - Netlifyにデプロイして、継続的に動作確認ができるようにする

## サポートブラウザ
WWA Wing に準拠します。

## ローカルで動かしたい
``` sh
# リポジトリをクローンしてください
$ git clone git@github.com:matsuyuki-a/wwa-next.git
## クローンしたリポジトリのディレクトリに入ります
$ cd wwa-next
## 依存しているライブラリをインストールします
$ npm install
$ npm run bootstrap ## 内部的に lerna bootstrap が呼ばれます
$ npm run build ## 各種ソースをコンパイルします
## 開発用のサーバを起動します (内部的にengine ディレクトリ下での npm startが呼び出されます。)
$ npm start
```

WWA Wing 本体のソースは `packages/engine/src` 下にあります。

## ブランチ戦略
- `develop` ブランチが最新です。

## ライセンス
- ソースコード: MIT (Expat) 
  - Original: WWA Wing Team https://wwawing.com/
- ドキュメント・画像・音源: CC-BY 4.0
