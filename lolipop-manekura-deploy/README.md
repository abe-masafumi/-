# loripop-manekura-deploy

[マネクラ](https://mc.lolipop.jp/)

[gitでloripopにデプロイ](https://github.com/abe-masafumi/git-deploy-)

ロリポップマネージドクラウドとGitHubのSSH通信設定まで参考にしていい↑

[ロリポの参考資料](https://support.mc.lolipop.jp/hc/ja/articles/360001503407

[ワンクリック鍵登録でダウンロードしたSSH秘密鍵を使用する](https://support.mc.lolipop.jp/hc/ja/articles/360052370234-%E3%83%AF%E3%83%B3%E3%82%AF%E3%83%AA%E3%83%83%E3%82%AF%E9%8D%B5%E7%99%BB%E9%8C%B2%E3%81%A7%E3%83%80%E3%82%A6%E3%83%B3%E3%83%AD%E3%83%BC%E3%83%89%E3%81%97%E3%81%9FSSH%E7%A7%98%E5%AF%86%E9%8D%B5%E3%82%92%E4%BD%BF%E7%94%A8%E3%81%99%E3%82%8B)

[sshファイルの権限](https://qiita.com/yuki82511988/items/0369808ad6cc226d936e)

エラー
```bush
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 48.70 KiB | 4.87 MiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Run node build process...
remote: 
remote: added 187 packages, and audited 188 packages in 22s
remote: 
remote: 18 packages are looking for funding
remote:   run `npm fund` for details
remote: 
remote: found 0 vulnerabilities
remote: 
remote: > kainushi-kentei@0.1.0 build
remote: > next build
remote: 
remote: info  - SWC minify release candidate enabled. https://nextjs.link/swcmin
remote: Attention: Next.js now collects completely anonymous telemetry regarding usage.
remote: This information is used to shape Next.js' roadmap and prioritize features.
remote: You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
remote: https://nextjs.org/telemetry
remote: 
remote: info  - Linting and checking validity of types...
remote: It looks like you're trying to use TypeScript but do not have the required package(s) installed.
remote: 
remote: Please install typescript and @types/node by running:
remote: 
remote:         npm install --save-dev typescript @types/node
remote: 
remote: If you are not trying to use TypeScript, please remove the tsconfig.json file from your package root (and any TypeScript files in your pages directory).
remote: 
remote: 
remote: > Build error occurred
remote: Error: Call retries were exceeded
remote:     at ChildProcessWorker.initialize (/var/app/.lolipop/build/node_modules/next/dist/compiled/jest-worker/index.js:1:11661)
remote:     at ChildProcessWorker._onExit (/var/app/.lolipop/build/node_modules/next/dist/compiled/jest-worker/index.js:1:12599)
remote:     at ChildProcess.emit (node:events:394:28)
remote:     at Process.ChildProcess._handle.onexit (node:internal/child_process:290:12) {
remote:   type: 'WorkerError'
remote: }
remote: Build seems to be failed. Abort
To ssh://ssh-1.mc.lolipop.jp:43962/
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://ssh-1.mc.lolipop.jp:43962/'

up to date, audited 416 packages in 604ms

97 packages are looking for funding
  run `npm fund` for details


found 0 vulnerabilities
```

このエラーはtypescriptのことが書いてある

解決策:
typescriptのバージョンを確認してlatestに変更した
nextのバージョンも変更した

#ロリポップ(マネクラ)のデプロイで詰んだところ

react-sheareがbuildエラーになる

twitterカードが表示されない

クーロンがよく壊れる

#ロリポのphpデプロイで詰んだところ

.envファイルを他のユーザーから隠す方法(600に設定変更)

.env内に[USER]を使用してはいけない。クーロン設定でエラーがでた


