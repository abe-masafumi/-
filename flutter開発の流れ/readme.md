# flutter開発の流れ

[flutter Document](https://docs.flutter.dev/)  

---
- flutterで使えそうな記事  
[flutter サンプルプロジェクト](https://flutter.github.io/samples/#)  
[flutter コンポーネント](https://gallery.flutter.dev/#/)  

- flutter環境構築  
使用するツール   
github  
androidStudio  
Xcode  
Sumilator  

> 以前にflutterを使ったことがあったので今回は途中から環境構築  
> flutter doctorで足りないものを追加した感じ  

**参考資料**  
[android studioとgithubを連結](https://www.mechengjp.com/%E3%80%90flutter%E3%80%91android-studio%E3%81%A8github%E3%82%92%E9%80%A3%E6%90%BA%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95/)  
[CocoaPodsの使い方を徹底解説](https://ios-docs.dev/cocoapods/)  
[CocoaPodsとは](https://guides.cocoapods.org/using/getting-started.html#installation)  

- flutterで開発

"androidStudio"でサンプルプロジェクトを作成  

[firebaseと接続](https://firebase.google.com/docs/flutter/setup?authuser=0&hl=ja&platform=ios#available-plugins)  

- "App Distribution"でテストアプリの配布
"App Distribution"画面で  
"ios"は"IPA"ファイルをアップロードしてください  
"android"は"apk"ファイルをアップロードしてください  

"Android App Bundle"って方法が推奨されているらしい  
[Android App Bundle](https://developer.android.com/platform/technology/app-bundle)

しかし"App Distribution"でアプリを配布するにはAPKで出力する必要がある？   

**IOS**  
```bush
flutter build ios --release
```
IPAファイルを作成のためにios版でbuildしようとしたらエラーが出た

参考資料  
[flutter build ipaコマンドを使ってみた](https://takamii.hatenablog.com/entry/2021/07/02/151453)

なんかXcodeとアップルIDを取得しろと言われた(すでに持っているけど)

参考資料  
[iPhoneアプリ開発環境の準備～Apple ID取得とX codeインストール](https://prokids.jp/article/iphone_pre)

エラー内容は先にappleで何か登録してください？って感じ？

```
flutter build ipa
```
このコマンドでもエラーが出る

[apple Developer account](https://developer.apple.com/account/)


**andoroid**  
```bush
flutter build apk" 
```

複数のエラーが出ながらもBuildが実行完了した。  
> "Built build/app/outputs/flutter-apk/app-release.apk"とか3つのファイルが自動生成される

apk
```bush
flutter build apk --split-per-abi
```

これでビルドしてできたファイルを"App Distribution"に貼り付けた  
ファイルの場所  "[project]/build/app/outputs/apk/release/app-armeabi-v7a-release.apk"  

<img src="app_Distribution001.png" width="600px">


- リリース  

[サヤパスが詰んでた⇨アップロード キーストアを作成する](https://docs.flutter.dev/deployment/android#signing-the-app)