
こんな想定

- ログインはメールアドレスでさせてログイン後に各種サービスとの連携をする
- ユーザー1人に対して複数のサービスとの関連付けを行う

---

全体の流れ

1. gemを追加
2. omniauthの設定ファイルを作る
3. Modelを作る
4. Controllerを作る
5. Viewを作る

---

Model

rails g devise:install
rails g devise User
rails g model Auth uid:string provider:string user_id:integer

---

Controller

rails g controller home index
rails g controller auth create destroy

---


