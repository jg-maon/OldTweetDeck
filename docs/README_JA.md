﻿# OldTweetDeck
昔のTweetDeckを取り戻しましょう！無料で！

> また、2015〜2018年のTwitterを取り戻したい場合は [OldTwitter](https://github.com/dimdenGD/OldTwitter) 拡張機能もチェックしてみてください。

![スクリーンショット](https://lune.dimden.dev/9713d947d56.png)

### 他の言語での説明
[English README](/README.md)  
[한국어 README](docs/README_KO.md)

## インストール方法

注意: 拡張機能ファイル(Chromiumの場合はZipファイルを展開したもの、Firefoxの場合はZipファイル)をインストール後に削除しないでください。

### Chromium (Chrome, Edge, Opera, Brave など) 

1. [リリースページ](https://github.com/dimdenGD/OldTweetDeck/releases) から `OldTweetDeckChrome.zip` をダウンロードする
2. Zipファイルを展開する
3. 拡張機能ページを開く (`chrome://extensions`)
4. デベロッパーモードを有効にする (拡張機能ページの右上に切り替えスイッチがあります)
5. "パッケージ化されていない拡張機能を読み込む"をクリックする
6. Zipファイルを展開したフォルダを選択する
7. https://twitter.com/i/tweetdeck にアクセスして昔のTweetDeckを楽しむ
8. [開発が継続できるように支援する](https://www.patreon.com/dimdendev)

### Firefox

#### Nightly / Developer Edition

1. [リリースページ](https://github.com/dimdenGD/OldTweetDeck/releases) から `OldTweetDeckChrome.zip` をダウンロードする
2. 高度な設定ページを開く (`about:config`)
3. `xpinstall.signatures.required` の設定を false に変更する
4. アドオンページを開く (`about:addons`)
5. アドオンページ右上の歯車アイコン→"ファイルからアドオンをインストール..."をクリックする
6. ダウンロードしたZipファイルを選択する
7. https://twitter.com/i/tweetdeck にアクセスして昔のTweetDeckを楽しむ
8. [開発が継続できるように支援する](https://www.patreon.com/dimdendev)

#### Stable

**Stableバージョンでこの拡張機能を使うことは推奨されません**

1. `about:debugging#/runtime/this-firefox`を開く
2. "一時的なアドオンを読み込む..."をクリックしてダウンロードしたZipファイルを選択する
3. **この方法でインストールした場合、Firefoxを閉じた際に拡張機能が削除されます**

### Safari

対応していません

## 更新

TweetDeckのファイルが更新された場合は、タブを再読み込みするだけで拡張機能を再インストールすることなく自動的に更新を受け取れます。 (`localStorage.OTDalwaysUseLocalFiles = '1'`の設定をしている場合を除く)  
拡張機能のファイルが更新された場合は、拡張機能を再インストールすることで更新を受け取れます。

## Better TweetDeck

この拡張機能と一緒に使うことが出来るBetter TweetDeckの[fork](https://github.com/dimdenGD/BetterTweetDeck/releases)を作りました。  
この拡張機能のインストール方法と同じ方法でインストールすることができます。

## よくある質問

#### 拡張機能が動かなくなりました

不具合報告をする前に、拡張機能を再度インストールしてみてください。

#### Manifest version 2 is deprecated, and support will be removed in 2023. という警告が表示されました

その警告は無視してください。  
   
#### ユーザーカラムや検索カラムが読み込まれません

API制限に達しているため読み込めていません。しばらくしてAPI制限が解除されるとまた表示されます。  

## 更新履歴

### 3.3.1
* フィルターを変更するとカラムが消える問題を修正

### 3.3.0
* OldTweetdeckが読み込まれない問題を修正
  * Twitterがカラムの位置と全体の状態を保存するAPIを削除したため、それらのAPIを再現しブラウザ内に状態を保存するようにしました
* **TweetDeckの状態がリセットされるため、更新前でTweetDeckを表示できている場合は検索クエリやカラムの配置をメモしておくことをおすすめします！**

**この拡張機能の開発を続けるために[寄付](https://dimden.dev/donate/)をご検討ください**

<details>
<summary>過去の更新履歴</summary>

### 3.2.3
* 複数アカウントでのリプライのフィルタリングに関する不具合を修正
* 日本語でツイートの展開が動作しない問題を修正

### 3.2.2
* フォローしていないアカウントへのリプライがホームタイムラインで表示される問題を修正
   * この挙動が気に入った人向けにオプションで切り替え可能にしました  
![](https://github.com/dimdenGD/OldTweetDeck/assets/26517362/7e4321aa-9320-4e83-92e3-a8b6d29a8109)

### 3.2.1
* いいねを読み込めるように修正
* いいねが動作するように修正
* コレクションを読み込めるように修正
* メンションを読み込めるように修正

### 3.2.0
* ホームタイムラインを読み込めるように修正
* リストを読み込めるように修正
* 通知が動作するように修正

### 3.1.9
tweetdeck.com のリダイレクトを修正

### 3.1.8
* ツイートをブックマーク (`Bookmark tweet`) ボタンを追加
* 三点リーダー (`…`) でハッシュタグとリンクが動作しなくなる問題を修正
* 長いツイートを表示するとリンクが失われる問題を修正

### 3.1.7
* API制限を緩和する機能を再び追加しました！  
![TweetDeckの設定ボタンから設定画面を開く](https://github-production-user-asset-6210df.s3.amazonaws.com/26517362/269732181-f3eb8979-a452-4080-bc50-a96d1cc41ed6.png)  
![Enable rate limit bypass (OldTweetDeck)をクリック](https://github-production-user-asset-6210df.s3.amazonaws.com/26517362/269732138-785187b2-fbdd-456f-b53e-007b9ab0b68f.png)

TweetDeckの設定ボタンから設定画面を開き、`Enable rate limit bypass (OldTweetDeck)`をチェックすることで有効にできます

API制限の緩和機能を利用する場合、以下の点にご留意ください
* API制限を受けた後に緩和機能を有効にした場合、OldTweetDeckは動作を再開するはずですが、Twitter Webはしばらくの間API制限が続く可能性があります
* API制限の緩和機能の利用はリスクが高くなります、自己責任でご利用ください
* この機能はしばらくテストされていないため、実際長期的にうまく機能するかどうか不明です
* 単なる理論的な考えですが、この機能を有効にしてもAPI制限を受けている場合、この機能を無効にするとAPI制限が解除される可能性があります

その他の更新内容
* 長いツイートを表示するためのボタンを追加
* 三点リーダー (`…`) が表示されない問題を修正
* 長いリツイートが正しく展開されない問題を修正
* 展開されたツイートの末尾にある`t.co`のリンクを削除するように修正

#### 3.1.6
バージョン更新

#### 3.1.5
長いツイートを表示するためのボタンを追加

#### 3.1.4
* ツイートを投稿できない問題を修正
* リツイートができない問題を修正
* ツイートが削除できない問題を修正
* リプライが正しく表示されない問題を修正

以下の機能はもう動作しません。  
* API制限の緩和
* アクティビティタブ

#### 3.1.3
リプライが表示されない問題を修正

#### 3.1.2
ツイートが削除できない問題を修正

#### 3.1.1
ツイートができない問題を修正

#### 3.1.0
READMEを更新

#### 3.0.8
バージョン更新

#### 3.0.7
日本語READMEを追加

#### 3.0.6
このバージョンではリクエストに傍受を追加しました。  
通常のTwitterをリバースエンジニアリングして、通常のTwitterで使用される対応するリクエストを見つけました。  
TweetDeckがシャットダウンAPIを使用しようとすると、リクエストは新しいエンドポイントにリダイレクトされ、結果は古いフォーマットに変換されます。  
  
ユーザーカラムと検索カラムがAPI制限の影響を受けるようになったことにより読み込めない問題を修正しました。  
最終的にはさらに多くのAPIが壊れることが予想されますが、その度に新しい動作するAPIに置き換えていく予定です。  
実行されるリクエストは通常のTwitterのリクエストと同じであるため、安全です。

#### 3.0.5
バージョン更新

#### 3.0.4
API上限を倍に緩和

#### 3.0.3
固定ツイートも表示するように変更 (最近のツイートの場合)

#### 3.0.2
複数アカウントのタイムラインに常にメインアカウントが表示される問題を修正

#### 3.0.1
バージョン更新

#### 3.0.0
リファラーを削除

#### 2.0.5
2.0.4で修正した問題がFirefoxで発生していたのを修正

#### 2.0.4
新TweetDeckが表示される場合がある問題を修正

#### 2.0.3
manifest V2 がFirefoxで動作しない問題を修正

#### 2.0.2
クリックが反応しない問題を修正

#### 2.0.1
新TweetDeckのheadとbodyを削除

#### 2.0.0
manifest V2 で作り直し外部サーバーを必要としないように変更

#### 1.0.2
恐らく動作する

</details>

## 日本語翻訳
[@katabame](https://twitter.com/katabame)  
以下の時点の内容を基に翻訳されています。  
* README: commit [294882a](https://github.com/dimdenGD/OldTweetDeck/commit/294882a3d5de029b2b1158d331c8549c941e34ac)  
* 更新履歴: release/tag [v3.3.1](https://github.com/dimdenGD/OldTweetDeck/releases/tag/v3.3.1)
