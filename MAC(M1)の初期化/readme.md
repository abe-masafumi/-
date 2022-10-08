 # MAC(M1)の初期化

  全てのデータを移行するだけならこの作業は必要ありません。[こちら](https://support.apple.com/ja-jp/HT204350)

 ---

 参考動画

 [M1 Macは初期化＆再インストール方法が違う](https://www.youtube.com/watch?v=VsYi4W7hkpY)

 初期化する間にやっておくべきこと

 [アップル公式](https://support.apple.com/ja-jp/HT201065)

 [【保存版】正しいMacの完全初期化方法 Macを売る前にやること](https://macgarage.jp/mac-initialize/)

 ---

### 自分のパソコンを整理整頓する
  
- [不必要なアプリケーションのアンインストール](https://www.lifehacker.jp/article/206045remember-to-delete-and-unlink-your-accounts-before-dele/)
- 画像、動画はハードディスクに保存しよう(TOSHIBA External USB 3.0 MediaのHDDを使用しているが現在のmacでは使用不可😭不便)
他の人も同じことが起きているM1チップのせいではないのかも。[こちら](https://www.buffalo.jp/support/faq/detail/1199.html)
[こっちも](https://soundorbis.com/mac-ex-hdd-ssd-fomat/)
HDDでは使用が困難でしたが、SSDなら問題なく使用できるかも知れない。アップル製品のために周りの環境も買い替えるの必要があるのはデメリット。
家にあるSDカードが使用できるか試した。問題なく使用できた。SDカードは幅広い機器で使用できるので容量の大きなSDカードを一つ持っておくと便利かも

> ついでにmacの悪口。iphoneの遠隔操作ができるツールが全然M1に対応してないからやりたいことができない。最近対応してないツール多すぎて辛い。nreal airもアップル製品の対応が微妙やし、外部ストレージ使えんし、アップルサポートに問い合わせしたらアップルシリコンに対応していないものは難しいの一点張り、究極のど素人が出てきてイラッとした。次はwindows買います。

- デスクトップを整理(必要なプロジェクトをgithubなどで管理してデスクトップからは削除)

### バックアップを作成

- [いざという時、元に戻せるように別のハードディスクにtime machineでバックアップ](https://support.apple.com/ja-jp/mac-backup)

- vscodeの設定忘れたw


### 機密情報管理 (同じパスワードを使い回しているものはこの際セキュリティーを高めるために、変更しよう)

- パスワード類は全てアナログで管理できるようにしておく(暗号化またはhash化したzipファイルをgoogledriveに保存でもいいかも)[メモ帳](https://news.allabout.co.jp/articles/o/27889/)

- [safariのパス](https://br.atsit.in/ja/?p=66244)、[google chromeのパス](https://yoshitechblog.com/google-chrome-password-information-confirmation)、[braveのパス](https://lv73.net/brave-password-control-where/)、[パソコンで管理しているパス(キーチェーン)](https://support.apple.com/ja-jp/HT211145#:~:text=Safari%20%E3%81%A7%E4%BF%9D%E5%AD%98%E6%B8%88%E3%81%BF%E3%81%AE%E3%83%91%E3%82%B9%E3%83%AF%E3%83%BC%E3%83%89%E3%82%92%E8%A1%A8%E7%A4%BA%E3%81%99%E3%82%8B&text=%E3%80%8CSafari%E3%80%8D%E3%83%A1%E3%83%8B%E3%83%A5%E3%83%BC%E3%81%8B%E3%82%89%E3%80%8C%E7%92%B0%E5%A2%83,%E3%81%99%E3%82%8B%E3%81%93%E3%81%A8%E3%82%82%E3%81%A7%E3%81%8D%E3%81%BE%E3%81%99%E3%80%82)

- [保存されたパスワードを一括エクスポートする方法](https://atmarkit.itmedia.co.jp/ait/articles/2006/03/news021.html#:~:text=%E3%83%91%E3%82%B9%E3%83%AF%E3%83%BC%E3%83%89%E3%82%92CSV%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AB%E4%BF%9D%E5%AD%98%EF%BC%88%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88%EF%BC%89%E3%81%99%E3%82%8B%E3%81%AB%E3%81%AF,-Chrome%E3%81%AB%E4%BF%9D%E5%AD%98&text=%E3%81%82%E3%82%8B%E3%81%84%E3%81%AFURL%E3%81%A8%E3%81%97%E3%81%A6%E3%80%8Cchrome%3A%2F%2F,%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88%EF%BC%BD%E3%82%92%E3%82%AF%E3%83%AA%E3%83%83%E3%82%AF%E3%81%97%E3%81%BE%E3%81%99%E3%80%82)

注意 Braveで溜まった仮想通貨を引き継ぐために準備しよう
今回Google Chrome感覚でBraveのパスワードのみ保存してましたが、仮想通貨の引き継ぎができませんでした。Choromeと違ってアカウントログインとかはしていなかったのが原因です。ウォレットに接続していたらもしかしたら引継ぎできてたかも？あとモバイルとの同期もできるので調べてみよう

- [保存されたパスワードを一括エクスポートする方法](https://atmarkit.itmedia.co.jp/ait/articles/2006/03/news021.html#:~:text=%E3%83%91%E3%82%B9%E3%83%AF%E3%83%BC%E3%83%89%E3%82%92CSV%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AB%E4%BF%9D%E5%AD%98%EF%BC%88%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88%EF%BC%89%E3%81%99%E3%82%8B%E3%81%AB%E3%81%AF,-Chrome%E3%81%AB%E4%BF%9D%E5%AD%98&text=%E3%81%82%E3%82%8B%E3%81%84%E3%81%AFURL%E3%81%A8%E3%81%97%E3%81%A6%E3%80%8Cchrome%3A%2F%2F,%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88%EF%BC%BD%E3%82%92%E3%82%AF%E3%83%AA%E3%83%83%E3%82%AF%E3%81%97%E3%81%BE%E3%81%99%E3%80%82)

> エクスポートしたCSVファイルは googleとbraveは共通のフォーマット,safariは少しフォーマットが違うので注意(エクスポートしたCSVファイルはインポートもできる)

### 必要なアプリケーションはスクショとっておくと良いかも(不必要なアプリケーションもあるので新しい環境では必要なものだけ再度インストールする方がいい)

- 設定の確認（マウスなどのカスタム設定）の設定画面をスクショしておくと良いかも

- 接続解除 (初期化したパソコンを再度自分で使用する場合は必要ない)

  iTunesからサインアウト

  iCloudからサインアウト

  iMessageからサインアウト

  Bluetoothデバイスの解除

### macOSの再インストール（初期化）

- M1マックは初期化手順が違うので注意！バグの原因になる

初期化はyoutubeを参考にしてください

[M1 Macは初期化＆再インストール方法が違う](https://www.youtube.com/watch?v=VsYi4W7hkpY)
 

### 初期化後の立ち上げ 

初期の立ち上げには1時間かかる

初期化後にパソコンを使用する場合はWifiが必要　パスワードの準備。

アップルアカウントのログインが必須になるので前もって準備する
今回はパスワードを忘れてしまい。再発行した。(パスワードを忘れた場合は再発行が必須)前もって準備しておくとスムーズ

### 立ち上げ後の設定

最初に環境設定を適用に自分好みにいじる

### 好みのブラウザをダウンロード

SafariはiCloudかアップルアカウントと紐づいてるらしい
パスワード、ブックマークもそのまま

Google Chrome ダウンロード
自分のアカウントでログイン
サイトに保存されているパスワードもアカウントに紐づいてるみたいで便利
ざっとみた結果Chrmeでやることは拡張機能のMetamaskの再設定だけかな

MetaMask
シンポリックリンクで再登録
ネットワークの追加(全部消える)
「モバイルと同期」ができるが現在使用不可なので後回し

Braveのインストール
Braveのアカウント引き継ぎできなかった
引き継ぎするための方法調べる
Braveで溜まった資産が消えたがそこまで重要じゃないからセーフ
Braveのウォレット追加
後で

Vscodeをインストール
拡張機能と設定は後で
https://zenn.dev/ryuu/scraps/4061aaee059d89

### コマンド類を使えるようにしたい。

homebrewで一気に揃える
https://zenn.dev/sawao/articles/e7e90d43f2c7f9

Githubとパソコンの連結(sshを前のパソコンから引き継ぐ)
https://tracpath.com/bootcamp/git-install-to-mac.html

今回は新しく作り直してみる
git コマンドは使えるがgitとの連結ができていないので連結する
https://mae.chab.in/archives/2306
https://zenn.dev/schnell/articles/0e1c2e9db5c08d

pythonのインストール
https://www.python.jp/install/macos/install_python.html
https://freeheroblog.com/brew-python/
https://gallard316.hatenablog.com/entry/2020/11/24/185634
homebrewでpythonをインストールしてもpipが使えなかったが安心してください

nodeのインストール


vscodeの設定





  

