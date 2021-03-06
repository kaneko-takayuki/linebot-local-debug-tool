Line Bot Development Tool
===
LineBot開発のための、ローカル上で挙動を確認することができるインターフェースツール

## Description
LineBotは、ユーザがメッセージ送信を送ることをきっかけに、あらかじめ設定しておいたサーバにアクセスし、返したいメッセージを求めてLine上に表示することで動いています。

そのため、Line上で自分の作ったBotを動かすためには、作成したサーバをWeb上にデプロイする必要があります。

しかし、それは開発中においては少し不便で、例えば少しずつ処理を変えて確認してみたいという場合には、毎回デプロイしなければいけず面倒臭いです。

そこで、ローカル上でも簡単にBotの挙動を確認できるツールがあれば便利だと思ったので、これを作成しています。

## Demo
※5/15(火)時点での挙動です。
![result](https://github.com/kaneko-takayuki/line-bot-development-tool/blob/media/gif/5-15_LineBotDemo.gif)

## Install
※あらかじめ、Nodeの環境構築を行い、`yarn`コマンドを使えるようにしてください。

- このリポジトリをクローンして、ディレクトリに入ります。

`git clone https://github.com/kaneko-takayuki/line-bot-development-tool.git`

`cd line-bot-development-tool`

- 次に、`yarn`コマンドで依存ライブラリをインストールします。(少し時間が掛かります。)

`yarn install`

- ビルドを行います。

`yarn build`

これで準備完了です。

## Usage
1. 本ツールはローカル上でLine Bot用のサーバとやり取りすることによって動作するので、サーバを起動させます。
2. 本ツールを`electron .`コマンドで起動させます。
