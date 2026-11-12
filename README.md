# MY FESTIVAL STUDIO — Web版

## GitHub Pages で公開する（無料）
1. GitHubにログインし、新しい **Public** リポジトリ `my-festival-studio` を作成します。公開するとコードとサイトは誰でも閲覧できます。
2. このフォルダの `index.html`、`manifest.webmanifest`、`icon.svg` をリポジトリの**ルート**にアップロードし、Commit changesします。ZIP自体をアップロードしないでください。
3. リポジトリの **Settings → Pages → Build and deployment** で Source を **Deploy from a branch**、Branch を **main**、Folder を **/(root)** にして Save。
4. 表示されたURL（通常 `https://ユーザー名.github.io/my-festival-studio/`）をSafariで開きます。反映まで数分かかる場合があります。
5. iPhoneでSafariの共有メニュー → **ホーム画面に追加** からアイコンを作れます。

## 更新する
ChatGPTから修正版の `index.html` を受け取り、GitHubの同名ファイルを置き換えます。URLは変わりません。

## データの扱い
編集内容はアクセスしたブラウザの localStorage に保存されます。端末間同期はありません。SafariのWebサイトデータを消去すると失われることがあります。変更前に「データをJSONで保存」でバックアップしてください。HTMLファイル版とWeb版は保存先が異なるため、自動で引き継がれません。旧版でJSONを書き出し、Web版で読み込んでください。

## Spotifyについて
この版にはSpotify連携は未実装です。Spotify API連携には別途Spotify Developerのアプリ登録、Client ID、HTTPSのRedirect URI設定、OAuth PKCEの実装が必要です。Client SecretをHTMLに書かないでください。
