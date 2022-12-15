# flutter開発の流れ

[flutter Document](https://docs.flutter.dev/)

---
[flutter サンプルプロジェクト](https://flutter.github.io/samples/#)

[flutter コンポーネント](https://gallery.flutter.dev/#/)




- flutter環境構築


使用するツール  
github  
androidStudio  
Xcode  
Sumilator  


以前にflutterを使ったことがあったので途中から  
flutter doctorで足りないものを追加した感じ

[android studioとgithubを連結](https://www.mechengjp.com/%E3%80%90flutter%E3%80%91android-studio%E3%81%A8github%E3%82%92%E9%80%A3%E6%90%BA%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95/)
[CocoaPodsの使い方を徹底解説](https://ios-docs.dev/cocoapods/)
[CocoaPodsとは](https://guides.cocoapods.org/using/getting-started.html#installation)


- flutterで開発

サンプルプロジェクトを作成

firebaseと接続  
https://firebase.google.com/docs/flutter/setup?authuser=0&hl=ja&platform=ios#available-plugins

- App Distributionでテストアプリの配布
App Distributionでアプリの配布

IOS   "flutter build ios --release"
IPAファイルをアップロードしてください。⇨IPAファイルを作成のためにios版でbuildしようとしたらエラー
https://takamii.hatenablog.com/entry/2021/07/02/151453  
内容は先にappleで何か登録してください？って感じ？
andoroid  "flutter build apk"
複数のエラーが出ながらもBuildが実行完了した。
```
Built build/app/outputs/flutter-apk/app-release.apk 
```

[apple Developer account](https://developer.apple.com/account/)

- リリース
