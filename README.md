# s3-history-mode

## 現状

- VueJSの遷移はHashモード(URLの語尾が/#/)での遷移のため、できればHistoryモード(URLの語尾が/)で遷移したい

## 理想

https://router.vuejs.org/ja/guide/essentials/history-mode.html

- S3でHistoryモードを実現したい(Apacheで言う所の、Rewrite設定を実現したい)

## テスト用ファイル

- /distにHistry設定がされているビルド済みのファイルが格納されている
  - /dist配下のファイルをS3に格納してテストする

## 正常な挙動

- /aboutにアクセスした時に、正常にページが読み込まれ、「This is an about page」と表示されること
- URLパラメータ(e.g. /about?test=test)を付与した時にも、パラメータが維持されながら遷移すること
