## usersテーブル

| Column             | Type   | Option   |
| ------------------ | ------ | -------- |
| email              | string | NOT NULL |
| encrypted_password | string | NOT NULL |
| nickname           | string | NOT NULL |
| birthday           | date   | NOT NULL |
| college            | string | NOT NULL |

### Association
 - has_many :users

## Classesテーブル

| Column    | Type       | Option            |
| --------- | ---------- | ----------------- |
| title     | string     | NOT NULL          |
| day_id    | integer    | NOT NULL          |
| number_id | integer    | NOT NULL          |
| teacher   | string     | NOT NULL          |
| text      | text       | NOT NULL          |
| comment   | text       |                   |
| user      | references | foreign_key: true |

### Association
 - belongs_to :user

アプリケーション名
みんなの時間割！

アプリケーション概要
時間割を簡単に管理できる

URL

テスト用アカウント
　メールアドレス
　
　パスワード
　
利用方法
時間割を登録して、自分の好きなようにカスタマイズできる

目指した課題解決
学生がわざわざログインしてネットを開き時間割を確認したり、紙を持ち歩き、時間割を確認しないようにするため

洗い出した要件


GIFと説明


実装予定の機能
フレンド機能
誰かが時間割を登録したらそれを自分のやつにも登録できる
小学生、中学生、高校生、大学生と時間割のビューを変えられる
自分で時間設定ができる

ローカルでの動作方法

