## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
* https://zipcloud.ibsnet.co.jp/api/search
  指定された郵便番号から、日本国内の都道府県・市区町村・町域を検索して返すAPI。
* リクエストとレスポンスのフォーマット
  https://zipcloud.ibsnet.co.jp/api/search?zipcode=1000001
  検索したい7桁の郵便番号
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
* エンドポイントと機能
  https://jsonplaceholder.typicode.com/users/1
  ユーザーIDを指定すると、そのユーザーの詳細情報（名前、メール、住所など）を取得できる。フロントエンド練習用に使われるダミーAPI。
* リクエストとレスポンスのフォーマット
* https://jsonplaceholder.typicode.com/users/3
* {
  "id": 3,                         // ユーザーID
  "name": "Clementine Bauch",     // 名前
  "username": "Samantha",         // ユーザー名
  "email": "Nathan@yesenia.net",  // メールアドレス
  "address": {
    "street": "Douglas Extension",  // 番地・通り名
    "city": "McKenziehaven",        // 市
    "zipcode": "59590-4157"         // 郵便番号
  }
}
### Q3-3. 感想
* 今回の課題で苦労したこと
  APIのレスポンス形式を事前に確認せずに表示処理を組んでしまい、undefinedエラーが出て原因を探すのに時間がかかった。
* 演習を通して理解できたこと
  fetchとawaitの基本的な使い方を理解できた
* Web APIの利便性や課題など
* Web APIは簡単に外部データと連携でき、さまざまなサービス構築に使えることが分かった
